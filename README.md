# Elasticity-Labs-1
Labs on Elastic Load Balancers

## Description
<P> Elastic Load Balancing allows the distribution of incoming traffic to your Amazon AWS infrastructure across multiple instances. This represents a great tool in avoiding failures in your applications and web traffic. ELB automatically detects fails in your EC2 instances and redirects traffic to other available instances. During this Lab, you will learn to create and use your first ELB instance to balance the HTTP traffic between two EC2 instances. You will also gain a valuable understanding of the Classic Load Balancer behavior during an instance outage.

### Step 1: Select a load balancer type

<P> Elastic Load Balancing supports different types of load balancers. For this tutorial, we shall create a Classic Load Balancer.</p>

### To create a Classic Load Balancer

<P>  1.Open the Amazon EC2 console at https://console.aws.amazon.com/ec2/.

2. On the navigation bar, choose a Region for your load balancer. Be sure to select the same Region that you selected for your EC2 instances.

3. On the navigation pane, under LOAD BALANCING, choose Load Balancers.

4. Choose Create Load Balancer.

5. For Classic Load Balancer, choose Create.

### Step 2: Define your load balancer

<P> You must provide a basic configuration for your load balancer, such as a name, a network, and a listener.

A listener is a process that checks for connection requests. It is configured with a protocol and a port for front-end (client to load balancer) connections and a protocol and a port for back-end (load balancer to instance) connections. In this tutorial, you configure a listener that accepts HTTP requests on port 80 and sends them to your instances on port 80 using HTTP.

### To define your load balancer and listener

1. For Load Balancer name, type a name for your load balancer.
 The name of your Classic Load Balancer must be unique within your set of Classic Load Balancers for the region, can have a maximum of 32  characters, can contain only alphanumeric characters and hyphens, and must not begin or end with a hyphen.

2. For Create LB inside, select the same network that you selected for your instances: EC2-Classic or a specific VPC.

3. [Default VPC] If you selected a default VPC and would like to choose the subnets for your load balancer, select Enable advanced VPC   configuration.
  
4. Leave the default listener configuration.
  
  ![ELB 1](https://user-images.githubusercontent.com/103466963/174758810-b1308400-ee9e-416c-8d62-b0c6b4060176.png)
  
