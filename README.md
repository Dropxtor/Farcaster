
## Prerequisites

- First, Buy A VPS which has 16 GB of RAM , 4 CPU cores or vCPUs, 40 GB of free storage
- Then, Visit [Infura](https://app.infura.io/)
- Setup Ethereum Mainnet and Optimism Mainnet RPC
- Copy Ethereum Mainnet & Optimism Mainnet RPC Endpoints


## Deployment


- Download [Termius](https://termius.com/download/windows) (I used termius for running node, but recorded this video in gitpod. Don't use gitpod)
- Connect your VPS then paste this command

```bash
wget https://raw.githubusercontent.com/Dropxtor/farcaster/main/node.sh && chmod +x node.sh && ./node.sh
```
After running this command, you will see a blank terminal -


Now enter this command :

```bash
curl -sSL https://download.thehubble.xyz/bootstrap.sh | bash
```
After that, it will ask for Ethereum RPC, Optimism RPC and then your farcaster username. Paste one by one


Once you will paste all those things,you will see something like this in your terminal


Boom, Your node is started !! After some times, you will see something like this in your terminal :


It means, your node is operational.

- Now press ```Ctrl+A+D``` to detach from the screen session safely


## FAQ

#### 1) Can I shutdown my PC after running this node?

Ans : Yes, that is why you are asked to  buy VPS, all these things will continue to happen in your VPS even after shutting down your PC / closing Termius or Putty App

#### 2) I have 16 gb ram in my PC, I do not want to buy VPS to run this node. Is it fine?

Ans : Yes, if you can run your PC all the time (24 hrs in a day 😁) without internet disruption . Actually it is not possible, that is why it is better to buy a VPS.

#### 3) I have 2 gb ram in my PC, But here the requirement is 16 GB. Then how can I run this node?

Ans : That is why you need to buy VPS of 16 GB. Even your pc has 2 gb ram but still you can run this node if u buy a VPS of 16 GB RAM.

#### 4) How can I again enter to my Farcaster node screen?

Ans : You need to run this command `screen -r farcaster` if you have followed my guide.

#### 5) My node is getting stopped, what to do?

Ans : Use this command `cd ~/hubble && ./hubble.sh upgrade`

#### 6) I'm facing this issue `crontab is not installed. Please install crontab first` . What to do?

Ans : Use this command `sudo apt install cron` and then again paste `curl -sSL https://download.thehubble.xyz/bootstrap.sh | bash`
