# Day One Notes 

Some interesting projects were mentioned in the various keynotes that are of interest to me.

## [Bare metal host provisioning for Kubernetes from RedHat](http://metal3.io/)

The Metal³ project (pronounced: Metal Kubed) exists to provide components that allow you to do bare metal host management for Kubernetes. Metal³ works as a Kubernetes application, meaning it runs on Kubernetes and is managed through Kubernetes interfaces.

* http://metal3.io/
* http://metal3.io/documentation.html

## [Thanos - Time Series Database](https://github.com/thanos-io/thanos)

Long term storage of Prometheus time series data. 

* https://github.com/thanos-io/thanos
* https://www.slideshare.net/FabianReinartz/storing-16-bytes-at-scale-81282712

## [Rook - Cloud Native storage for Kubernetes](https://rook.io/)

### Storage Operators for Kubernetes
Rook turns distributed storage systems into self-managing, self-scaling, self-healing storage services. It automates the tasks of a storage administrator: deployment, bootstrapping, configuration, provisioning, scaling, upgrading, migration, disaster recovery, monitoring, and resource management.

Rook uses the power of the Kubernetes platform to deliver its services via a Kubernetes Operator for each storage provider.

### Multiple Storage Providers
Rook orchestrates multiple storage solutions, each with a specialized Kubernetes Operator to automate management. Choose the best storage provider for your scenarios, and Rook ensures that they all run well on Kubernetes with the same, consistent experience.

### Rook and Ceph 

Rook uses Ceph for distributed file system.

## [MinIO - High Performance Object Storage](https://docs.min.io/)

It is API compatible with Amazon S3 cloud storage service. Use MinIO to build high performance infrastructure for machine learning, analytics and application data workloads.

* https://docs.min.io/docs/minio-gateway-for-s3.html
* https://docs.min.io/docs/minio-gateway-for-azure.html
* https://docs.min.io/docs/minio-gateway-for-nas.html
* https://docs.min.io/docs/deploy-minio-on-kubernetes.html


