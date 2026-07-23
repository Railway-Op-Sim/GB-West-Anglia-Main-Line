# West Anglia Main Line

The West Anglia Main Line is a busy route running from London Liverpool Street to Cambridge.

This simulation covers the West Anglia Main Line from Harlow Town to Cambridge North, as well as the Stansted Airport branch, and part of the Cambridge line from Cambridge to Meldreth.

A variety of stopping, semi-fast and express services operate along the route, as well as the occasional freight service. All junctions along the route are flat junctions, making for some very busy areas.

## Simulation

A timetable for spring 2022 has been included, running from 04:00 until 03:59 the next morning (although few services operate overnight).
The standard off-peak service frequencies are as follows:

### Greater Anglia

- 2tph Stratford to Bishop's Stortford
- 2tph London Liverpool Street to Cambridge North
- 1tph Cambridge to Ipswich
- 1tph Norwich to Stansted Airport

### Stansted Express

- 2tph London Liverpool Street to Stansted Airport

### Great Northern

- 1tph London King's Cross to Ely
- 1tph London King's Cross to King's Lynn

### Thameslink

- 2tph Brighton to Cambridge
- 1tph London King's Cross to Cambridge

### CrossCountry

- 1tph Birmingham New Street to Stansted Airport

Some additional services operate in peak hours (particularly to King's Lynn), and some of freight services operate to various destinations along the route throughout the day.

A large portion of these routes use multiple speed limits - a higher limit for passenger multiple units and a lower limit for loco-hauled freight services. As this is not possible to replicate in ROS, only the higher speed limit has been included. As such, freight services often end up running early. Be careful not to route them ahead of passenger services which may get stuck behind them later on. Don't be afraid to use the passing loops to let a freight train wait for its correct schedule again!

## Operational Tips

### Cambridge

- Platform allocations have been provided - while it is not essential to follow these it is recommended to avoid getting trains stuck.
- To access platform 4 from the south (London/Stansted) direction, it is recommended to route the train around platform 1 rather than through it. Due to the nature of ROS, the train will stop at the first platform it encounters so if it is routed through platform 1 it will stop there instead.
- Most trains (particularly from the south) have several minutes of extra "pathing" time added in to their schedules - as such they will arrive at Cambridge early. Sometimes they can be routed in on arrival, however sometimes it may be preferable to hold them outside the station to wait for other platforms to clear. This is particularly the case when the arrival is headed for platform 4, but a train from platforms 7 or 8 needs to depart south - these moves can not happen at the same time.
- Be wary of where you make trains wait around Cambridge - especially to the north. There are very few signals and it is extremely easy to block everything up without realising. This is especially problematic after about 22:30, when trains are returning to the sidings.
- Keep an eye on destinations - during peak hours some Cambridge North services terminate at either Cambridge or Ely instead. Additionally, trains from Birmingham New Street and Norwich terminate at Cambridge instead of Stansted Airport in the early morning and late evening.
- Be wary of which direction points are set. When setting a route the program will try and find a route that follows the directions points are switched first, and will prioritise changing the last set of points first. As such, given the small number of signals, it is very easy to route a train across both lines, blocking parallel moves. It is recommended to manually set points back to normal by clicking them after a train has passed to avoid routes being set like this accidentally.

### Stansted Airport

- Platform allocations have been provided - while it is not essential to follow these it is recommended to avoid getting trains stuck.
- Trains typically have several minutes extra "padding" time on arrival at Stansted Airport - particularly those from the north. It may be necessary to hold trains on the mainline or before the single track stretch to allow a departure first.
- Be careful with the bidirectional lines into the station - depending on how the points are set you an end up with some interesting routes!

### Bishop's Stortford

- Trains terminating at Bishop's Stortford use platform 3 - this is the bottom platform in the simulation.
- Terminating services will often arrive early and it may be preferable to hold them on the mainline to allow a Stansted Express service through back towards London.

### Harlow Town

- Some trains are overtaken at Harlow Town (particularly the Bishop's Stortford services) - these have long dwell times at Harlow Town and should be routed into the outer two platforms while express services pass through the middle.