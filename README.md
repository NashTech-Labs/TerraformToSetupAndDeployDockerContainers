This template will explain help to set up and deploy Docker containers using Terraform.

Once Docker is installed, for our demo purposes, we will need to expose the daemon without TLS. Go to the Docker Desktop for Windows settings and make sure ‘Expose daemon on TCP:localhost:2375 without TLS’ is ticked. Apply the settings and Docker will restart.

We will be using the Docker provider as found on the Terraform registry:

Note for reference to connect to a Linux or macOS-based machine with Docker installed you would use the host line:


- Run `terraform init` on the directory that holds the configuration file
- Run `terraform plan`
- Then `terraform apply`

- using `docker container ls` you can see the container running


To cleanup, type `terraform destroy` .