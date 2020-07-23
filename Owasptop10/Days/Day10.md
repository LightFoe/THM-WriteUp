# Day 10
## Insufficient Logging and Monitoring

This rooms ends with a warning, you should always log everything, indeed melius abundare quam deficere overall if we're talking about retrieve information abount an attack a site 
had received or to prevent it.
They put lots of emphasis on loggin and they're right; as the final test you'll check a log from an attempted attack on a web server

![](/images/day10/logs.png "logs")

There is indeed in the logs some unauthorized login attempts ( to /login) with different common credential.
The ip is an easy find and the first answer is gone, the second one is on the type of this attack. It's trying different passwords commonly known and, probably, it's not even using a wordlist beacuse there were only 4 login attempts ... It's like bruteforcing the way in ... let's try to guess what is the attack type :smirk:
