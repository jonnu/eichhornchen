Entities to consider
--------------------

* user (abstract, login core)
* user_customer
* user_operator
* address
* machine
* machine_type (e.g. custom, production machine, rostock, i3, i2, mendelmax, blah)
* machine_rating
* machine_capability
* machine_operator (link operator to machine, many to many)
* message
* material (e.g. PLA, ABS)
* location (a GEOIP cache table)
* object
* job
* job_status
* MAYBE  - amount earned for community competition?
         - amount spent into community (internel only?)

Schema
------

TBA

Job Flow
--------

When the job has an operator & machine, and everything is agreed, the flow should be something along the lines of:

# JOB_CREATED
# JOB_QUEUED
# JOB_PRINT_INPROGRESS
# JOB_PRINT_COMPLETE
# JOB_SHIPPING_PENDING
# JOB_SHIPPING_COMPLETE
# JOB_COMPLETE

Error statuses:

* JOB_FAILED
