## Setting up the tool on a VM on GCP

### Prerequisites (for setting up on GCP):
- GCP account for setting up the VM
- Enable Billing for your project on GCP

### Prerequisites(for setting up on Local system)
- Any OS(Ubuntu, Windows, Mac)
- 8GB RAM
- 40GB free HD space
- Docker 
- Docker-Compose

**Note**: *Since setting up these tools on local system may slow downs the processing of the system, I am setting it up on GCP VM for better performance.*

## Steps to setup the tool
- Step 1: Signup or Signin to your GCP account
- Step 2: [Create a project in the GCP account ](https://cloud.google.com/resource-manager/docs/creating-managing-projects)
- Step 3: Now we will create the VM in our newly created Project using Google's [Compute Engine Service](https://cloud.google.com/compute) with the below configuration:
    - Machine Configuration:
        - Machine Family: General-purpose
        - Series: N1
        - Machine type: n1-standard-4(4 vCPU, 15GB Memory)
    - Boot Disk:
        - Public Images
        - OS: Ubuntu 18.0.4 LTS
        - Boot disk type: Standard persistent disk 
        - Size: 50GB
    - Identify and API access:
        - Service account: Compute Engine default service account
        - Access scopes: Allow default access
    - Firewall
        - Allow HTTP traffic
        - Allow HTTPS traffic
     
        
        


