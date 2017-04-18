# Ubuntu Image

The Ubuntu GKE image is an image optimized to run Kubernetes on the Google
Cloud Platform.

The image is currently made to behave as much as possible like the GCI image,
but since it uses "real" systemd (instead of upstart with a delegate), the systemd
targets need to be changed slightly to ensure services are always started on
boot.
