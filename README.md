swift-sum
=========

Calculates the checksum of the object (md5) including the SLO and DLO segment caluclations 
<http://docs.openstack.org/developer/swift/overview_large_objects.html>
<http://docs.openstack.org/developer/swift/misc.html#slo-doc>

usage: swiftsum [-h] [-s SEGMENT_SIZE] [-r READ_SIZE] filename [filename ...]

Calculates the checksum of the object including SLO and DLO segments.

usage: swiftsum [-h] [-s SEGMENT_SIZE] [-r READ_SIZE] [--slo] [--dlo] [-v]
                filename [filename ...]

Calculates the checksum of the object including SLO and DLO segments.

positional arguments:
  filename              file name to check

optional arguments:
  -h, --help            show this help message and exit
  -s SEGMENT_SIZE, --segmentsize SEGMENT_SIZE
                        File segment size (default: 500M)
  -r READ_SIZE, --readsize READ_SIZE
                        Segment size to read from disk (default: 40Mi)
  --slo                 Calculate the SLO (Static Large Object) checksum
                        (default).
  --dlo                 Calculate the DLO (Dynamic Large Object) checksum.
  -v, --verbose         Verbose (default: off).
