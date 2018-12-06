# foglamp-filter-delta
FogLAMP C++ "delta" filter passes deltas of reading data. A new reading
is only sent onwards if the value of one or more data points in the new
reading differs fromthe previous reading sent by the specified tolerance
percentage.

By defining a minimum rate it is possible to force readings to be sent
at that defined rate regardless of the change in value of the reading.

Rates may be defined as per second, per minute, per hour or per day.

 Configuration items
  - tolerance	The percentage tolerance when comparing reading data
  - minRate		The minimum rate at which readings should be sent
  - rateUnit	The units in which minRate is define (per second, minute, hour or day)
