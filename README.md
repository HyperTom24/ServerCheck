ServerCheck
===========

This is a project for a console application which examines local disk space, searches how many windows updates there are (important and optional), and examines the event log for errors and warnings.  This only works on Windows systems.  It is something I was doing for work, but I'd like it to be my first repository example.

This is a VB.NET Console Application.  If you intend to use it, you can follow this outline (taken from part of the program's output)...

----------------------
SERVERCHECK.EXE [-DS] [-WU] [-EL] [-SC] [-GN] [-LB]
  -DS    Check for free disk space.
  -WU    Check for windows updates.
  -EL    Check the event log.
  -SC    Suppress console output during program execution.
  -GN    Generate new EventLogFilters.CSV file.
         NOTE: Using -GN will override default program functionality
         by ONLY generating a new CSV (unless other argument checks are specified)
  -LB    Look Back specification. This will overwrite the default EventLog lookback of 31 days to whatever number is specified.
         NOTE: If using -LB you MUST input a positive integer afterward.
  
  Specifying any of the first 3 flags above will override default program functionality by checking ONLY what is specified in the program argument list.
----------------------
