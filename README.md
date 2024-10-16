# FYP
Final Year Project(UCD, 2023-2024)
The term "Internet of Things" (IoT) describes a network that connects various objects to the
internet using predefined protocols. This network relies on information-sensing devices to facilitate
the data interaction and communication. Its purpose is to enable intelligent functions such as
recognition, positioning, tracking, monitoring, and management[1]. Internet of Things(IoT) has
gradually coming into people’s life in recent years. As the development of intelligent devices,
these devices are connected via network to provide convenience for people’s life. However, large
amount of data generated by IoT devices needs to be processed by devices that with efficient
resource allocation and low latency. Edge technology processes data as close as possible to its
physical source[2]. Therefore, Edge-computing becomes one of the possible solutions that is able
to provide low latency services to end-users. Distributed nodes usually have limited computing and
storage resources compare to Cloud resources, and they can be accessed with higher bandwidth
and less latency as distributed nodes usually more close to mobile users[3], however, the limited
computing and storage resources of distributed nodes cause resource shortage and higher latency
with the increasing number of users. In those scenarios where the users move across different edge
servers and migrate users’ modules across different edge servers, the destination server selection
becomes extremely important, because this is closely related to providing low-latency services,
it also affects the users’ experience. Low-latency is the key requirement of latency-sensitivity
application, such as Cardiovascular Health Monitoring(CHM) used in this project. After user
moves to a new place, the selection of destination server usually affect the performance of latencysensitivity application. In other words, in order to decrease the latency between servers and
users, modules require to be dynamically deployed on new low latency destination devices as users
move, to improve the performance of latency-sensitivity application, this is presented as migration
challenge. This project mainly focus on low latency new destination edge node selection for the
mobile user. In the iFogSim2 built-in algorithm, whenever the user moves to a new destination,
the device that is the closest to the user is selected as new destination. My initial strategy was to
enhance the built-in algorithm by introducing dynamic clustering and load-balance so that the new
destination device was selected based on resources status of different candidate servers rather than
simply selecting the closest one. So, an algorithm called Resources-based Dynamic Clustering Load
Balance(RLB) has been proposed. RLB aims to improve latency between fog nodes and end users.
The algorithm integrated within the iFogSim2 has been used as benchmark against the proposed
algorithm in this report, these two algorithms have been evaluated and compared in this report
based on different test cases. The main goal of this project is to enhance the selection of new
target edge device, to find new parent device with low latency and provide better experience to
mobile user. To benchmark these improvements, we use the built-in default algorithm to compare
with the algorithm presented in this report.
