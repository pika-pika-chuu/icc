# icc
A series of tools &amp; tutorials for internet censorship circumvention

## Prerequisite
- A Virtual Private Server (VPS)
- V2Ray/Vmess server app
- Content Delivery Network (CDN) provider for your VPS
- Mobile application for connecting to your VPS

Follow the steps below in order.

## Architecture
![Arch](https://github.com/pika-pika-chuu/icc/blob/main/arch.jpg?raw=true "arch")


### 1. Virtual Private Server (VPS) setup
These are the two main options. Choose **either**:
- AWS EC2
- Digital Ocean Droplet


#### AWS EC2
1. Register for an AWS account: [Setup and Secure AWS Free Tier Account](https://www.youtube.com/watch?v=FRQ9fE4fd5g)
2. Create an AWS EC2 instance [How to Create AWS EC2 Instance](https://www.youtube.com/watch?v=k_FPNHUh66A)

#### Digital Ocean Droplet
1. Create a Digital Ocean account. It will ask you to pay for $5 if using paypal which can be later used in your account: [Create Digital Ocean Account](https://cloud.digitalocean.com/registrations/new)
2. Create a Droplet: [How to Create a Droplet](https://www.youtube.com/watch?v=kzThZOZj1S4)

### 2. Setup your V2Ray server
In your EC2 or Droplet instance, follow the instructions provided in the following repository: [Xray server](https://github.com/SonyaCore/V2RayGen)

### 3. Place the server behind a CDN
You can find a list of avaliable free CDN providers at [Free CND List](https://geekflare.com/free-cdn-list/). Here we use **Cloudflare** as the CND of our choice: [How to Setup Cloudflare Free CDN?](https://www.youtube.com/watch?v=N7n_HtvwNVA)

### 4. Download the client apps for your mobiles or PCs
Here you can find the list of files for every platform available. You will use the settings you set in step 2 of this instructional: [v2ray-core releases](https://github.com/v2ray/v2ray-core/releases)

#### Other available apps
- **Android**:
  1. Google Play Store: [v2rayNG](https://play.google.com/store/apps/details?id=com.v2ray.ang&hl=en_AU&gl=US)
  2. Files and binaries: [v2ray releases](https://github.com/2dust/v2rayNG/releases)
- **IOS**: [Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118)

### More resources
Visit [Project V](https://www.v2ray.com/en/) and [Shadowsocks](https://github.com/shadowsocks) for more resources.
