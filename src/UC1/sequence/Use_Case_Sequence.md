# Assisted Rider-RideCar Rendezvous Sequence

## Description

## Request Phase
- Rider makes ride request to Omniverse
- Ominverse requests Rider's Position
- Omniverse queries for potential RideCars near Rider's Position for availability
- If none, then Omniverse reports to Rider and Done
- Omniverse makes RideRequest to query results with potential RideCars
- ForEach potential RideCar in results 
-    	If Omniverse receives positive response within time allowed, then confirm Ride with RideCar
-    	Else continue with next potential RideCar
- End
- If Ride confirmed, Omniverse reports Confirmation to RideCar and to Rider
- Else Omniverse reports Failure to Rider and Done
## Approach Phase
- Async: Omniverse requests that Rider and RideCar start providing Pose reports. On receiving a Rider Pose, the RideCar is notified. On receiving a RideCar Pose, the Rider is notified. Whenever the distance between the Rider and RideCar is less than the VisibilityLimit, the Omniverse places a virtual Sign Posed above the RideCar and a virtual Sign Posed above the Rider.
## Meeting Phase
- Whenever the RideCar has a Pose that would support pickup of the Rider, the Omniverse flashes the virtual Signs and notifies the Rider and RideCar.
## Completion Phase
- When the RideCar notifies the Omniverse that the Rider has been accepted into the RideCar, the Omniverse takes down the virtual signs.
 