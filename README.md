# Swarm-role
Swarm role and Tg bot guide

# 1. Install Go

```
cd ~
wget go.dev/dl/go1.24.0.linux-amd64.tar.gz
sudo rm -rf /usr/local/go
sudo tar -C /usr/local -xzf go1.24.0.linux-amd64.tar.gz
```
```
echo 'export PATH=$PATH:/usr/local/go/bin' >> ~/.bashrc
echo 'export GOPATH=$HOME/go' >> ~/.bashrc
echo 'export PATH=$PATH:$GOPATH/bin' >> ~/.bashrc
source ~/.bashrc
```
check installation
```
go version
```
# 2. Setup Tg bot
2.1
Go To t.me/BotFather

Send /newbot and follow the instructions:

It will Ask You to enter the Name & username of the Bot:

Now it will send the Token. Look Like this: 84100000:AAGITsRXgxxxxNuP56-xxxxxxxxxxxxxxx ( dont share it with anyone ) imp

# 2.2 Get Your Chat ID:

head to your bot which was created and send message:

Visit: https://api.telegram.org/botYOUR_BOT_TOKEN/getUpdates

Dont Forget to replace YOUR_BOT_TOKEN with your: which we create in above step:

You will see your Id here : Save it:

Note: If you get an empty result {"ok":true,"result":[]}, you may need to send a message to your bot first, then refresh the URL and you will get it

# Install Gswarm node 
```
go install github.com/Deep-Commit/gswarm/cmd/gswarm@latest
```
check version
```
gswarm --version
```
 Configure GSwarm:
```
gswarm
```
Enter Your BotToken from
Enter Your ChatId From
Enter Your EOA address From Gensyn Dashboard with your gensyn Mail

 # Link Dc & Telegram
1. Get the verification code From Discord
In Gensyn Dc go to swarm-link channel

Enter /link-telegram

You will get your code from here

2. Verify the code in Telegram Bot
Go to Your bot which you created

type /verify {code} , Replace code with your actual one which u got from DC

After verify your code You will automatically get your Role
Done 🎉