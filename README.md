1 - 14 Line: Specify keypair and AIM type.  
15 - 25 Line: Create VPC element  with Vpc1 name under Resources element.
26 - 42 Line: This element creates Public Subnet,giving as a ref our VpcId,has  different CIDR range than Vpc Cidr range.
43 - 59 Line: Define Private Subnet with ref name as Vpc1  and different range than previous CIDR range.
60 - 66 Line: Internet gateway element with "IgwVpc1" Id is important for Vpc to connect to Internet. 
67 - 73 Line: Previous element Internet Gateway to attach Vpc .
74 - 80 Line: This will be Public Route Table for the first created Vpc.
81 - 89 Line: On this block specify our Public Route Table's path.
90 - 96 Line: Subnet Association config for Vpc1PublicRouteTable
97 - 103 Line: Private Subnet Table created.
104 - 111 Line:Create a NAT gateway,we must specify the public subnet in which the NAT gateway should reside. 
112 - 116: Allocated Elastic IP.
117 - 126: This block will deploy the second VPC named Vpc2.