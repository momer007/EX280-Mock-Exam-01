# EX280
EX280 Mock Exams 01

Performance-Based Exam: Managing OpenShift Container Platform

Instructions:

This exam consists of practical tasks that you need to perform on an OpenShift cluster.
You are required to complete the tasks using the provided environment.
Ensure that all configurations persist after a cluster reboot without intervention.
You have 2 hours to complete the exam.
Feel free to use the OpenShift web console, command-line interface, and product documentation as needed.

Task 1: Manage OpenShift Cluster

	1.1. Use the web console to create a new project named "mock-exam-project".

	1.2. Use the command-line interface to create a service account named "admin-user" with cluster-admin role.

	1.3. Verify the status of the cluster and list all running pods in the "mock-exam-project" project.

	1.4. View the logs of the pod named "nginx-deployment-xyz" in the "mock-exam-project" project.

	1.5. Monitor cluster events and identify any critical alerts. Take appropriate action to resolve them.

Task 2: Deploy Applications

	2.1. Deploy an application named "wordpress" using the provided WordPress template.

	2.2. Scale the WordPress deployment to have 3 replicas.

	2.3. Create a new deployment named "job-runner" using the provided job.yaml file to perform a one-time task.

	2.4. Expose the WordPress service externally to port 8080 using an OpenShift route.

	2.5. Configure MetalLB operator to manage load balancing for the WordPress service.

Task 3: Manage Storage for Application Configuration and Data

	3.1. Create a secret named "database-creds" with username and password for MySQL database.

	3.2. Provision a PersistentVolumeClaim named "app-data" with a storage class named "standard".

	3.3. Mount the "app-data" volume to the WordPress deployment to store uploaded media files.

	3.4. Configure StatefulSets to use non-shared storage for MySQL database.

Task 4: Configure Applications for Reliability

	4.1. Configure liveness and readiness probes for the WordPress deployment.

	4.2. Set resource limits for CPU and memory for the WordPress deployment.

	4.3. Implement horizontal autoscaling for the WordPress deployment based on CPU utilization.

Task 5: Manage Authentication and Authorization

	5.1. Configure HTPasswd identity provider for authentication.

	5.2. Create a new user named "exam-user" with a password "exam123".

	5.3. Assign the "exam-user" to the "edit" role within the "mock-exam-project".

Task 6: Configure Network Security

	6.1. Generate TLS certificates for securing external traffic to the WordPress service.

	6.2. Create a network policy to restrict traffic to the WordPress deployment.

	6.3. Configure an external route named "wordpress-route" to expose the WordPress service.

Task 7: Enable Developer Self-Service

	7.1. Configure resource quotas for CPU and memory for the "mock-exam-project".

	7.2. Implement a project quota limiting the number of pods in the "mock-exam-project".

	7.3. Create a project template for deploying PHP applications.

Task 8: Manage OpenShift Operators

	8.1. Install the MySQL operator into the cluster.

	8.2. Delete the Elasticsearch operator from the cluster.

Task 9: Configure Application Security

	9.1. Create a service account named "privileged-user" with elevated privileges.

	9.2. Apply security context constraints to restrict access for the "privileged-user".

	9.3. Create a secret to store sensitive information such as database passwords.

Task 10: Configure Kubernetes CronJobs

	10.1. Create a CronJob named "backup-job" to back up the WordPress database daily.

	10.2. Verify that the "backup-job" is scheduled correctly and inspect its logs.

Task 11: Update OpenShift

	11.1. Update the OpenShift cluster to the latest available version.

	11.2. Identify any deprecated Kubernetes API usage and update relevant resources.

	11.3. Update the installed operators to their latest versions.
