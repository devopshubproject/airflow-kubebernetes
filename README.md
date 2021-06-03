# airflow-kubebernetes
This Project contains the script (Kubernetes mainfest files) to deploy the HA cluster.

# **Airflow**

### **What is Apache Airflow**

| Airflow Platform created by the community to programmatically author, schedule and monitor workflows.

Use Airflow to author workflows as Directed Acyclic Graphs (DAGs) of tasks. The Airflow scheduler executes your tasks on an array of workers while following the specified dependencies

### **Principles**

* Dynamic
* Extensible
* Elegant
* Scalable

### **Use Case of Airflow**

Airflow is not a data streaming solution. The Workflows are expected to be mostly static or slowly changing.

### **Running Airflow**

Airflow can be installed and run by two methods:
1. Local Installation
2. Docker Installtion

As a third options we also get ready-made managed solution like MWAA in aws etc.,.

### **Airflow with Kubernetes**

Kubernetes gives an advantage in your environment, especially if you are optimizing app dev for the cloud, is that it gives you the platform to schedule and run containers on clusters of physical or virtual machines (VMs).

Let's see the bunch of advantages we get on running Airflow over Kubernetes.

#### _Scalability_

Airflow runs one worker pod per airflow task, enabling Kubernetes to spin up and destroy pods depending on the load.

#### _Resource Optimization_

Kubernetes spins up worker pods only when there is a new job. Whereas the alternatives such as celery always have worker pods running to pick up tasks as they arrive.