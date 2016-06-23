Then, type in the following command into your SSH Terminal:
  
   ```git clone [PASTE YOUR LINK HERE]```

Now you should have a **mean_adsk** folder in the folder structure, which is located on the left-hand side of the container. If you don't see it, you need to right-click the the container and click **refresh**. 

![](http://i63.tinypic.com/52yzyq.jpg)


Within the terminal, navigate to the mean_adsk folder by entering the following command: 

  `cd mean_adsk`


Then run the following commands: (Note: you may get an error, don't worry)
 
   `git branch -r | grep -v '\->' | while read remote; do git branch --track "${remote#origin/}" "$remote"; done`
   
   `git fetch --all`
