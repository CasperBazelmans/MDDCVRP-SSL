<instance_name> <n_veh_types> <n_number_vehs> <n_sls> <n_nodes>

[Vehicle Types]
ID_veh_type		Index of vehicle type (k)				(index)
Fixed cost 		Cost of using vehicle type				(euro)
Variable cost	Cost of driving 1 km with vehicle type		(euro/km)
Speed			Avg speed of vehilce type (k)				(km/h)
Capacity		Total capacity tax weight of vehicle type 	(quantity)
Alpha			Mixing level of vehicle type		 		(quantity)
Beta			Collect up to level of vehicle type			(quantity)
Max time		Total time the vehicle can be away from depot 	(seconds)
Max drive time	Total drive time of the vehicle			(seconds)

[Number of vehicle types]
ID_veh_type		Index of vehicle type (k)				(index)
ID_depot 		Index of depot (s)					(index)
# vehicles		Number of vehicles of this type (s,k)		(#)

[Scheduled lines]
ID_from		Depot index of departure				(index)
ID_to			Depot index of arrival					(index)
Cost per req	Cost of one piece on a scheduled line		(euro/req)
Capacity		Capacity of the scheduled line in tax weight	(quantity)
Departure time 	Departure time of scheduled line			(seconds)
Arrival time 	Arrival time of scheduled line			(seconds)

[Nodes / shipments]
ID_node		Node index							(index)
ID_depot		Assigned depot						(index)
Latitude		Latitude							(coordinate)
Longitude		Longitude							(coordinate)
Type			Type node							("depot" OR "collect" OR "distribute")
Service_time	Service time (10 min + 2 min per piece)		(seconds)
q_del 		Quantity to deliver					(quantity)
q_col 		Quantity to collect					(quantity)
tw_depot_start	Shipment available at depot				(seconds)
tw_depot_end 	Shipment deadline at depot				(seconds)
tw_cust_start	Start time window at customer				(seconds)
tw_cust_end		End time window at customer				(seconds)