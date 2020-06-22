# Waste Labs: GPS analysis

Contained in `data/` is a day's worth of GPS data of a waste collection fleet. The vehicles service both residential and commercial areas.

We want to estimate when the vehicles are collecting waste, using only their GPS records.

When they service commercial areas, the vehicles stop at locations while loading a large container. They can therefore stand-still for some-time.

When collecting residential waste, the vehicles slowly travel through a road-segment.

Each row in the data contains the following key information:

* `time`: time of GPS records
* `lon`-`lat`: the longitude and latitude position of the GPS records
* `WasteVehicles_idWasteVehicles`: unique identifier of the waste vehicle that generated the GPS records

All the other records can be ignored.

## Instructions

Choose one vehicle to analyse, and use any method to infer when the vehicle collected waste and when it was just travelling. You may calculate any features that you deem useful, such as speed or distance between consecutive points, and you can use advanced methods, such as DBSCAN, or simple rule-based methods.

You can choose if you want to analyse a residential collection vehicle, or a commercial collection vehicle.

The data is not labelled, so you will have to use other means to try and validate your results. This can include graphical inspection.

Package your results as python-notebook, which clearly describes the method that you chose to implement, your motivation for doing so, the results, and the results validation.

Share your results as a github project with a clear README.MD of where everything can be find. Also include a `pip` generated `requirements.txt` file that lists all the libraries required to run the notebook.

The only other requirement is that you have to use pandas in your analysis.

## Notes

Note that the sampling time of the records is quite low, at 1 minute between records. The records are not currently ordered.
