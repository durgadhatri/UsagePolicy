# OCI Resource Usage Policy

### Overview

OCI Resource Usage Policy is used to monitor the cores and clusters of OCI resources that are predefined for a user.

### Prerequisites

- Before adding the OCI Resource Usage Policy in the Template, ensure you have the following prerequisites:      
  
  Admin access to [CloudLabs Admin Portal](https://admin.cloudlabs.ai/) (If access is unavailable, kindly reach out to your point of contact or [CloudLabs Support](https://docs.cloudlabs.ai/RequestSupport)).

### Adding OCI Resource Usage Policy

1. Log in to the CL portal and navigate to the required tenant (WIZ). On the left-hand side of the page, you will see the Template section.

2. Navigate to the **Templates (1)** section in the left menu and click on the **edit (2)** button.

   ![](./img/01.png)

3. Scroll down to the **Usage Policy** section and provide the Usage Policy URL for the respective OCI resource. 
   
   ![](./img/02.png)

4. Then, click the **Submit** button.

   ![](./img/03.png)

### Usage Policy Uand Alerts Outputs

- Below are the Resource Usage Policy and Alerts outputs for the respective resources.

  1. Instance: Created more than one instance, but the usage policy had restrictions that allowed the creation of only one instance.

     - Policy:

      ```
      [
        {
          "ResourceType": "OCI.Instance",
      
          "Parameter": [
            {
              "Name": "max-ocpu-cores",
      
              "Value": "1"
            },
      
            {
              "Name": "max-memory-gb",
      
              "Value": "32"
            },
      
            {
              "Name": "max-instance-count",
      
              "Value": "1"
            }
          ]
        }
      ] 
      ```

     - Output:
       Cloud Screenshot: 

       ![](./img/04.png)

       ![](./img/05.png)
      

      
