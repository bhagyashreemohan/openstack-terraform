# openstack-terraform
This sample template will initialize your single openstack VM's 
further changes will be made for this repo
your comments are welcome.

OpenStack is an open source platform, which offers powerful virtual servers and required services for cloud computing. It is mostly deployed as Infrastructure-as-a-service (IaaS), which aims to provide hardware tools and components for processing, storage, and networking resources throughout a data center.
OpenStack Architecture

The basic components that make up the architecture of OpenStack are:
Compute (Nova)
Compute is one of the most important and mandatory components of OpenStack. It is basically a virtualization hypervisor. In a cloud computing environment, it acts as a controller, which manages all the resources in a virtual environment. It is also used to manage the high-performance bare metal configurations.
It is coded in Python and has utilized many pre-defined libraries to deliver robust functioning. The hypervisor technologies that might be used are Xen, KVM, and VMware and this selection, depends on the version of OpenStack used. SQL is used for database access.
Functionality
The nova-api handles the requests and responses from and to the end user.
The nova-compute creates and destroys the instances as and when a request is made.
Nova-scheduler schedules the tasks to the nova-compute
The glace registry stores the details of the image along with its metadata.
The Image store, stores the images predefined by the admin/user.
The nova-network ensures the network connectivity and routing.
Networking (Neuron)
This is responsible for establishing a neuron structure between the components for better connectivity. It manages all the networking related functionalities of the architecture as a whole. Starting from assigning and managing the IP addresses of the nodes to managing and implementing routing, it constitutes all.
Image
The instances of the virtual machines or the disk image are stored as images in the image storage Glance.
Object Storage (Swift)
This is the mountable storage unit of the architecture. It helps in data replication across the data center. The files and objects can be copied to multiple units with the help of this unit. The object storage units are replicated with every new server addition. It also stores the replicate content from all the active nodes and makes it available to the new clusters, ensuring a backup in case of any hardware failure or server loss.
Block Storage (Cinder)
Block Storage provides persistent level storage facilities for cloud-oriented computing devices. It helps in the creation, addition, and removal of the new block devices in the server. It provides complete integration with the OpenStack, reducing the use of extraneous hardware components. It can be accessed and instructed using CLI or web-based services. Linux based systems can go with Cloudbyte, EMC, Coraid, SAN Storage, etc.
When you are configuring your OpenStack cloud, you can choose the message broker and the database solution from a list of products/solutions available from the market, such as RabbitMQ, MySQL, MariaDB, and SQLite.


OpenStack can be accessed on web User Interface through CLI or through API calls using tools like curl or other plug-ins. Ultimately, all these REST API calls will issue access to the OpenStack services.
