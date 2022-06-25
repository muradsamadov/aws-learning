# EC2
EC2 have a 4 type:
1. On-Demand - for ex: you are use vm 10 hours and pay onle 10 hours. When poweroff vm payment stopped.
2. Reserved Instance "RI" - you are reserve range of time. For ex: this vm work 09:00-18:00
3. Spot - you are 10$ and this vm work only 10$. If it exceeds 10$ poweroff vm.
4. Dedicated Host - aws seperate only you dedicated Host.
# EC2 options
Elastic Block Store (EBS):
1. Volumes - similar to ESXI volumes. This stage add new volume. And this volume attach after instances. This stage add raids and after configure instances. When instance remove this volumes not remove. After you are use this volumes. This volumes make create snaphot
2. Snapshots - similar to ESXI snaphot but there are create snaphot only poweroff vm. This snaphot you are creae AMI and this AMI after you are create similar to before vm. AMI similar to ESXI template. This is a best way to create same configurations with old instance.
# EC2 Load Balancing
this options similar to haproxy. For example you are two node and app working bot nodes 80 port. And LoadBalancing configure that requests are send public loadbalancer ip 80 port forward this request two nodes 80 ports.
1. Load Balancers - create loadbalancer and add 'Target Groups'. To 'Load Balancers' configure which port listen, healthcheck and other. At the end you are copy 'Load Balancers' DNS name and use it. This is only dns name not have ip address.
2. Target Groups - this option configure which port listen to nodes, which instance forward and other
# Auto Scaling
This feauture similar to kubernetes autoscaling. For example if nodes cpu working more than 30% create 2 instance. Below features possible create it: 
Launch Configurations
Auto Scaling Groups