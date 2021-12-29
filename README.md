# pre.sh
Automated Presearch Bot Written In Bash 

Presearch is an open, decentralized search engine that rewards community members with Presearch Tokens for their usage, contribution to, and promotion of the platform.

[Presearch Website](https://presearch.org/)
[CoinMarketCap](https://coinmarketcap.com/currencies/presearch/)

Pre.sh script uses xdotool to automate mouse and keyboard movements and input.

# Running Pre.sh script as Cronjob

Pre.sh Script can be ran as a cronjob when the system starts. Pre.sh uses xdotool to automate mouse movement and keyboard input to run xdotool as a cronjob when the system starts we need to export the current display you can check the number that x has assigned to your display using command.

```
cat /proc/$$/environ | tr '\0' '\n' | grep '^DISPLAY='
```

```
#export display
export DISPLAY=:0

#export xauthority
export XAUTHORITY=/root/.Xauthority/
```

# Get Mouse Location With Xdotool

```
xdotool getmouselocation
```



