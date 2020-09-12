# Leak report

_Memory errors happen because when we use calloc the bytes don't free before we exit causing a leak of memory that is not being allocated You fix the code by adding free() to a spot in which the data stops being allocated In this case the free goes at the end of the iscleaned method but we have to put an if statement in because if we pass free an empty array it will fail._
