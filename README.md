swift-sum
=========

Calculates the checksum of the object (md5) including the SLO and DLO segment caluclations 
<http://docs.openstack.org/developer/swift/overview_large_objects.html>
<http://docs.openstack.org/developer/swift/misc.html#slo-doc>

usage: swiftsum [-h] [-s SEGMENT_SIZE] [-r READ_SIZE] [-v]
                filename [filename ...]

Calculates the checksum of the object including SLO and DLO segments.

positional arguments:
  filename              file name to check

optional arguments:
  -h, --help            show this help message and exit
  -s SEGMENT_SIZE, --segmentsize SEGMENT_SIZE
                        File segment size (default: 1Gi)
  -r READ_SIZE, --readsize READ_SIZE
                        Segment size to read from disk (default: 40Mi)
  -v, --verbose         Verbose (default: off).