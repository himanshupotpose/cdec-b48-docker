
# 🚀 Docker 

## 🔹 Monolithic vs Microservices
Monolithic :-
📖 Definition
Monolithic Architecture is a software architecture style in which the entire application is built as a single, unified codebase.
All components such as UI, business logic, and database access are tightly coupled and deployed together as one unit.

🔹 Key Characteristics :-

🧱 Single codebase
🔗 Tightly coupled components
🚫 Difficult to scale individual features
🔁 Single deployment process

Microservices :-
📖 Definition
Microservices Architecture is an architectural style in which an application is divided into small, independent services,
each responsible for a specific business functionality and communicating with other services through APIs.

🔹 Key Characteristics :-

🧩 Independent services
🚀 Easy and flexible scalability
🔄 Independent deployment
✅ Better fault isolation

### 📌 Traditional vs Vertualization vs Containerization
Traditional :-
📖 Definition
Traditional Deployment is a method where an application is installed and run directly on a physical server or operating system without any abstraction layer.

🔹 Key Characteristics :-

🖥️ Runs directly on the host OS
⚙️ Manual installation and configuration
❌ Environment dependency issues
🐢 Slow deployment and scaling

🖥️ Virtualization :-
📖 Definition
Virtualization is a technology that allows multiple Virtual Machines (VMs) to run on a single physical server using a hypervisor, where each VM has its own operating system.

🔹 Key Characteristics :-
🧠 Each VM has a separate OS
⚙️ Managed by a hypervisor (VMware, VirtualBox)
🐘 Heavy resource usage
⏳ Slower startup compared to containers

📦 Containerization
📖 Definition
Containerization is a lightweight virtualization technique where applications run in isolated containers while sharing the host operating system kernel.

🔹 Key Characteristics :-
🚀 Lightweight and fast
🐳 Uses Docker or similar tools
🔁 Consistent environment across systems
⚡ Starts in seconds

🐳 What is Docker?

📖 Definition
Docker is an open-source containerization platform that allows developers to build, package, and run applications inside lightweight, portable containers.

Docker ensures that an application runs consistently across all environments — from a developer’s laptop to production servers.


⚙️ Installation of Docker (Ubuntu / EC2)


📌 Follow the steps below to install and verify Docker on an Ubuntu-based system

🔄 Update System Packages
sudo apt update

📦 Install Docker Engine
sudo apt install docker.io -y

▶️ Start Docker Service
sudo systemctl start docker

🔁 Enable Docker on System Boot
sudo systemctl enable docker

🔍 Check Docker Service Status
sudo systemctl status docker

🐳 Verify Docker Installation
docker --version


🐳 Docker Commands

📌 Commonly used Docker commands to run, manage, monitor, and debug containers

docker run [IMAGE]                  
# Create and run a container from an image

docker run -d [IMAGE]               
# Run a container in detached (background) mode

docker ps                           
# List all running containers

docker ps -a                        
# List all containers (running + stopped)

docker create [IMAGE]               
# Create a container without starting it

docker start [CONTAINER_ID]         
# Start an existing (stopped) container

docker stop [CONTAINER_ID]          
# Stop a running container

docker rm [CONTAINER_ID]            
# Remove a stopped container

docker rm -f [CONTAINER_ID]         
# Force remove a container (running or stopped)

docker run -p [HOST_PORT]:[CONTAINER_PORT] [IMAGE]
# Map a container port to a specific host port

docker run -P [IMAGE]               
# Expose all container ports on random host ports (32768–61000)

docker exec -it [CONTAINER_ID] bash 
# Access the running container terminal

docker logs [CONTAINER_ID]          
# View container logs

docker stats [CONTAINER_ID]         
# View real-time CPU & memory usage




















