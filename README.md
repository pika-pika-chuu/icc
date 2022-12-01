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
2. Create an AWS EC2 instance: [How to Create AWS EC2 Instance](https://www.youtube.com/watch?v=k_FPNHUh66A)

#### Digital Ocean Droplet
1. Create a Digital Ocean account. It will ask you to pay for $5 if using paypal which can be later used in your account: [Create Digital Ocean Account](https://cloud.digitalocean.com/registrations/new)
2. Create a Droplet: [How to Create a Droplet](https://www.youtube.com/watch?v=kzThZOZj1S4)

### 2. Setup your V2Ray server
In your EC2 or Droplet instance, follow the instructions provided in the following repository: [Xray server](https://github.com/SonyaCore/V2RayGen)

### 3. Place the server behind a CDN
You can find a list of avaliable free CDN providers at [Free CDN List](https://geekflare.com/free-cdn-list/). Here we use **Cloudflare** as the CDN of our choice: [How to Setup Cloudflare Free CDN?](https://www.youtube.com/watch?v=N7n_HtvwNVA)

### 4. Download the client apps for your mobiles or PCs
Here you can find the list of files for every platform available. You will use the settings you set in [step 2](https://github.com/pika-pika-chuu/icc/edit/main/README.md#2-setup-your-v2ray-server) of this instructional: [v2ray-core releases](https://github.com/v2ray/v2ray-core/releases)

#### Other available apps
- **Android**:
  1. Google Play Store: [v2rayNG](https://play.google.com/store/apps/details?id=com.v2ray.ang&hl=en_AU&gl=US)
  2. Files and binaries: [v2ray releases](https://github.com/2dust/v2rayNG/releases)
- **iOS**: [Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118)

#### Sending client apps to blocked users
Most likely, the users behind the censored networks are unable to download these apps. There are multiple ways to transfer these files:
- E-mail attachments (Gmail, Yahoo, etc.) for small binaries `>25 MB`.
- File hosting services (Google Drive, Dropbox, etc.) for large binaries `<25 MB`.

These methods are better used in combination with [File encryption](https://github.com/pika-pika-chuu/icc/edit/main/README.md#file-encryption).

##### File encryption
Binary files will most likely be blocked by email and file hosting services and flagged as *malicious files*. To mitigate this issue, you need to **encrypt** these files:
- Zip in Windows: [Encrypt and password-protect ZIP files](https://www.pcworld.com/article/422788/how-to-encrypt-and-password-protect-zip-files-the-right-way.html)
- Zip in MAC: [Encrypt Zip File on Mac](https://www.winzip.com/en/learn/tips/encrypt-zip/mac/)

#### Install apps in iOS using iTunes
Unlike Android, iOS apps do not release their apps as files/binaries. If users cannot access the **App Store** on their iPhones, they need to install the app through iTunes on their PC or laptop:
1. Download [v2ray-core releases](https://github.com/v2ray/v2ray-core/releases) for Windows or Mac.
2. Zip and encrypt the file as explained in [File encryption](https://github.com/pika-pika-chuu/icc/edit/main/README.md#file-encryption).
3. Attach the zip file to your email or upload it to your Google Drive and share it with the intended user.
4. Now the user need to configure the software as explained in [step 2](https://github.com/pika-pika-chuu/icc/edit/main/README.md#2-setup-your-v2ray-server).
5. Follow **part 1** of [this](https://www.leawo.org/entips/download-and-install-iphone-apps-from-computer-1361.html) tutorial and search for [Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118).
6. The app is now transferred to your iPhone and can configure the Shadowrocket app using [step 2](https://github.com/pika-pika-chuu/icc/edit/main/README.md#2-setup-your-v2ray-server).


### More resources
Visit [Project V](https://www.v2ray.com/en/) and [Shadowsocks](https://github.com/shadowsocks) for more resources.
