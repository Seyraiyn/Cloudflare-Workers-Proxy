# Cloudflare Workers Proxy 
(google translated)

This is a simple reverse agent script based on Cloudflare Workers, which is used to forward the request of the client to the target address and return the response of the target address to the client. Before using this script, be sure to read the following safety precautions and disclaimers in detail to ensure safety and legal compliance when using the script. 

-Group chat: [HeroCore](https://t.me/HeroCore) 
-Channel: [HeroMsg](https://t.me/HeroMsg) 

![ image](https://github.com/user-attachments/assets/72b35862-16cc-4224-89e1-ad0419a7ac4e) 


## Introduction 

This Cloudflare Workers script acts as a reverse agent. Its main function is to receive the request from the client, and to represent the request to the target address, and then return the response from the target address to the client. Specific functions include: 

-Agent client requests to the target address. 
-Modify that the relative path in response is an absolute path to ensure the correct loading of resources. 
-Handle reorientation and make appropriate modifications to maintain the correctness of the resource path. 
-Add CORS head to allow cross-domain access. 

## How to deploy 

The following are the detailed steps for deploying Cloudflare Workers reverse proxy scripts: 

1.  Registration Cloudflare Account: If you do not yet have a Cloudflare account, please register an account on the official website of [Cloudflare ](https://www.cloudflare.com/). 

2.  Create Workers scripts: After logging into the Cloudflare account, enter the "Workers" section and create a new Workers script. 

3.  Copy [worker.js](worker.js): paste the provided reverse proxy script into the Workers editor. 

4.  Save and deploy: After saving the script, click the "Deep" button to deploy your Workers script. 

5.  Configuration domain name: In Cloudflare, associate your domain name with the deployed Workers script. Make sure to pass the traffic to your Workers script. 

6.  Test: Visit your domain name or Cloudflare Workers URL will see an input box in which you can enter the URL of the target website to be represented, and then click the "Enter Agent" button for access. 

## Method of use 

To use this reverse agent to visit other websites, please follow the following steps: 

1.  Send a request: Just send a request to your Cloudflare Workers URL and send the request to the target website. 

   Example request: `https://your-worker-url.com/https://example.com/` 

   Replace `your-worker-url.com` with your Cloudflare Workers URL, `example.com` with the address of the target website you want to represent. 

2.  Process reorientation 

   Reverse proxy scripts can handle reorientation and modify resource paths appropriately to ensure accuracy. 

3.  Allow cross-domain requests 

   The reverse agent added CORS (cross-source resource sharing) head to allow cross-domain requests. This means that you can initiate a request from a different domain (different domain name) in the front JavaScript code without being subject to cross-domain security restrictions on the browser. 

4.  User-friendly interface 

   If you do not provide URL for the target website, this reverse agent also provides a user-friendly interface. Users can enter the URL of the target website in this interface, and then click the "entry agent" button to quickly access the target website. 

## Precautions 

-Please ensure that the deployed Workers scripts are valid at the time of deployment and have sufficient resources to process the request. 

-Please be careful not to abuse the service to ensure that it is only used for legal and suitable purposes. 

## Disclaimer 

-**Liability limitation**: The author is not responsible for any safety issues, data losses, service interruptions, legal disputes or other damages that may result from the script. The use of this script requires its own risk. 

-** Improper use**: Users need to understand that this script may be used for illegal activities or unauthorized access. The author strongly opposes and condemns any improper use of scripts and encourages the use of legal compliance. 

-**Legality**: Please ensure compliance with all applicable laws, regulations and policies, including but not limited to Internet use policies, privacy regulations and intellectual property laws. Make sure you have legal authority over the target address. 

-**Self-risk**: The use of this script requires self-risk. The author and Cloudflare are not liable for the misuse, improper use or any damage caused by the script. 

**This disclaimer is aimed at non-mainland Chinese users. If used in mainland China, it is necessary to abide by relevant regional laws and regulations, and the users shall bear the corresponding risks and responsibilities themselves. ** 


## Resources 

-[Cloudflare Workers Document ](https://developers.cloudflare.com/workers) 
-[Cloudflare Workers Set ](https://developers.cloudflare.com/workers/platform/settings) 

## License 

This project uses MIT licenses. For details, please refer to the [LICENSE](LICENSE) file. 

Thank you for your use! If you have any improvements or suggestions for this project, you are also welcome to contribute codes or ask questions. 
