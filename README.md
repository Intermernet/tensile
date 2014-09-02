tensile
=======

Tensile Web Stress Test Tool

Example usage:

    $ tensile -help
    Usage of tensile:
      -c=5: Maximum concurrent requests (short flag)
      -concurrent=5: Maximum concurrent requests
      -cpu=4: Number of CPUs
      -e=1: Maximum errors before exiting, -1 for unlimited (short flag)
      -maxerror=1: Maximum errors before exiting, -1 for unlimited
      -r=50: Total requests (short flag)
      -requests=50: Total requests
      -u="http://localhost/": Target URL (short flag)
      -url="http://localhost/": Target URL
    

    
    $ tensile -concurrent=200 -requests=1000 -cpu=2

            Tensile web stress test tool v0.1
    
    Target URL:     http://localhost/
    Requests:       1000
    Concurrent:     200
    Processors:     2

    Waiting for replies...
    
    Replies:        1000
    Total size:     14.65KB
    Total time:     1.9903687s
    Average time:   1.990368ms



    $ tensile -c=200 -r=100

            Tensile web stress test tool v0.1

    NOTICE: -concurrent=200 is greater than -reqs
            Changing -concurrent to 100
    

            Tensile web stress test tool v0.1
    
    Target URL:     http://localhost/
    Requests:       100
    Concurrent:     100
    Processors:     4

    Waiting for replies...
    
    Replies:        100
    Total size:     1.46KB
    Total time:     197.1718ms
    Average time:   1.971718ms

*WARNING: This tool can rapidly deplete system resources with too many concurrent workers*