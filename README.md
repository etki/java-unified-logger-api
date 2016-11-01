# Huge prependous disclaimer:

This is not even a work-in-progress project, this is idea-in-progress 
project.
 
# Unified Logger API

This project is devoted to common problem of reconfiguring logger at 
runtime.

In most situations, you will be just happy with specifying proper 
`logback.xml` or something similar, and, maybe, rescan it every N 
seconds. However, if you distribute your project, run it cross-platform
or dump logs via network to addresses that may change at runtime - then
you're stuck, so this unified logger API comes to help you, acting as a
like slf4j little brother: it gives you common interface to manage 
appenders, targets, rolling policies and stuff.