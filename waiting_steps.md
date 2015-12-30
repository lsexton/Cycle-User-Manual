# Waiting Steps

Cycle is able to run the Steps within a Feature File rapidly. Often, the software that Cycle is testing does not respond as fast as Cycle can perform Steps. This variance is resolved by the use of Waiting Steps within Cycle. Waiting Steps are Steps that have an option to wait a designated length of time.  The amount of time that a Step will wait is specified in milliseconds or MS. 1 second is equal to 1000 milliseconds.

There are many Step in Cycle that can wait. The simplest waiting Step is I wait <number> ms which pauses the Feature File execution for the specified length of time. This Step can be used when you know a specific amount of time will allow the software being tested to be prepared for the next Step. A pause of 2000 milliseconds is typically enough time for an application to complete an operation. 

A common waiting Step when performing graphical screen interaction is I see <Image> within <Number> ms. This command will continue to scan the screen until the Image is found. Once the image is found, the execution continues. If the image is not found within the amount of milliseconds specified, the Step fails.
