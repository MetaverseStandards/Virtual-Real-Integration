# Assisted Rider-RideCar Rendezvous Sequence

## Use Case Description
A person (the Rider), walking in an urban area asks for a car (the Ride Car) to provide a ride. If a Ride Car is available, it is sent to the meet the Rider. When the Ride Car is close enough to the Rider for them to be mutually visible, a virtual signs appear over both the Rider and Ride Car to help them find each other. These signs face each other, rotating and moving in synchronization with the Rider and Ride Car until rendezvous has been achieved at a safe location for a pickup. Arrival at a safe location for pickup is indicated by a change in the appearance of the signs. At all times, the signs appear visually as the would if they were physical signs in the real world.

## Request Phase
1. Rider sends **Ride-Request** to Omniverse with a current Pose and waits for **Ride-Response**.
2. Omniverse sends Omniverse an **AvailableRideCars-Request** with Rider's Pose and waits for **AvailableRideCars-Response**.
3. If **AvailableRideCars-Response** is empty, then Omniverse sends a negative **Ride-Response** reports to Rider and the Rendezvous sequence is completed with status **Failure**. 
4. Omniverse re-sends Rider's **Ride-Request** with Pose to all RideCars identified in the **AvailableRideCars-Response** and waits until a timeout expires or a positive **Ride-Response** is received from some RideCar.
5. Omniverse sends **ConfirmRide-Request** to Rider and a **ConfirmRide-Request** to the responding RideCar and waits for **ConfirmRide-Response** (positive) from both Rider and RideCar. 
## Approach Phase
1. Omniverse sends Rider a **StreamPose-Request**, sends RideCar a **StreamPose-Request** and does not wait. 
2. Subsequently, when the Omniverse receives a Rider **Pose-Report**, the RideCar is receives a copy and when the Omniverse receives a RideCar **Pose-Report**, the Rider is receives a copy. 
3. Whenever the Omniverse determines that distance between the Rider and RideCar is less than the Omniverse-determined **VisibilityLimit**, the Omniverse sends a **Display-Request**(on) to the virtual Sign Posed above the RideCar and also to the virtual Sign Posed above the Rider. Access to the integrated content is mediated by the Omniverse.
## Meeting Phase
1. Whenever the Omniverse determines that the RideCar and Rider have Poses that would support pickup of the Rider, the Omniverse sends a **Flash-Request** to each of the virtual Signs.
2. The Omniverse also sends a **PickupPossible-Notification** the Rider and sends a **PickupPossible-Notification** to the RideCar.
## Completion Phase
1. When the Rider determines that they are picked up, the Rider sends a **Pickup-Notification**(completed) to the Ominverse.
2. When the RideCar determines that the Rider is picked up, the RiderCar sends a **Pickup-Notification**(completed) to the Ominverse.
3. If the Omniverse receives both **Pickup-Notification**(completed) messages, the Rendezvous sequence is completed with status **Success** and the Omniverse sends a **Display-Request**(off)to the virtual Sign Posed above the RideCar and also to the virtual Sign Posed above the Rider.

 