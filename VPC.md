# Virtual Private Cloud (VPC)
VPC is a aws network. This option configure network settings: \
1. Your VPC - create your vpc means to create your network. For ex: 10.10.0.0/16 network \
2. Subnets - create you subnets. For ex: 10.10.10.0/24 , 10.10.11.0/24 .. \
3. Route tables - means to for ex: when you are connect 10.10.0.0/16 network go to local, when are connect 0.0.0.0/0 network got to internete gateway. \
4. Internet gateways - this options you are connect internet and attact to vpc and this subnets ip address became public ip address. \
5. elastic ip - public instantes when reboot ip address changed. Through this options create one ip and allocation it. Then allocation public instances. Consequantly public instance have a only one ip address.
6. NAT gateways - maybe private instances connect to public and download or update something. Thats why we are create nat gateway and add route tables. This situation private instance connect to internet over nate gateway. Second part we are create nat instance and add route table. Nat gateway and nat instaces this difference: nat gateway expensive and only managed by amazon but nat instances you are create own and managed it you ; with nat instance allow to internet speed more than 48 mb/sec but nat gateway lower 48 mb/sec speed.
7. Endpoint - normally you want to connect  instance to s3 this connect must be public internet. But with endpoint you are connect locally to s3.
8. Peering Connections - maybe you are two different VPC and this vpc by default not are connected together. Through this option two different vpc can be connected together. For ex: 10.10.0.0/16 network can be connected to 10.20.0.0/16 network