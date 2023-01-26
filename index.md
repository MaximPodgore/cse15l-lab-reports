**First Step:**  


Please go to this [site](https://sdacs.ucsd.edu/~icc/index.php). It's a UCSD site for finding your specifc CSE15L account username (you might use it in other classes) and we're going to use this account to access a remote computer on a ucsd server.

Please put **your** information in like below  

![image](https://maximpodgore.github.io/cse15l-lab-reports/img1.png)  

Then, try to remember or copy down the last 3 letters of that additional accounts username. The password of it should be your tritonlink password. You'll find out if it works in a later step. If you do have to come back to this and reset it, make sure you disable the option that also resets your tritonlink password.  

![image](https://maximpodgore.github.io/cse15l-lab-reports/img2.png)  

Above and below are the two sections of the page you see once you look up your account

Next, click on [this](https://code.visualstudio.com/) to go to vscode's site and download it. It's an excellent IDE for most languages

![image](https://maximpodgore.github.io/cse15l-lab-reports/img3.png)  

Next, please click the install button and it should automatically give you the right version for your OS

**Second Step:**  

Open VS Code, locate the top bar, click on Terminal, and then select new Terminal. Like so  

![image](https://user-images.githubusercontent.com/56902053/214762802-a67f502a-7397-40fc-9b11-4fac39289f97.png)  

![image](https://user-images.githubusercontent.com/56902053/214762893-9ec54187-db96-4dcd-8202-7a811aa64ac9.png)

Put this in the Terminal, but substitute afs with the last 3 letters of your username (remember?)
`ssh cse15lwi23afs@ieng6.ucsd.edu` 

(here it is so you can copy and paste but please substitute those last 3)

![image](https://maximpodgore.github.io/cse15l-lab-reports/img4.png)  

When it works, this should pop up, type yes and click enter

![image](https://maximpodgore.github.io/cse15l-lab-reports/img5.png)  

Then input your Tritonlink password to be logged into the server
Once you're in you should see this  

![image](https://maximpodgore.github.io/cse15l-lab-reports/img6.png)  

**Third Step:**  

Now you're going to goof off in in the terminal since it is a useful tool for navigating remote computers and servers  

Click [here](https://opensource.com/article/22/5/essential-linux-commands) for some essential linux commands  

Here's a quick breakdown of some useful ones:  

`pwd` prints youre working directory  

`cd~` changes your directory to the root folder  

`ls` shows the contents of the directory you're in  

`cd <directory` allows you to change directories (go down the rabbit hole)  

`cd ..` allows you to go out of one folder back to one step before  

`touch` makes an empty file  

`mkdir` allows you to make a directory  

`cat` opens a file

`vi` allows you to write in the file. It's kinda hard to use the text editor so here's a cheat sheet if you're a masochist https://vim.rtorr.com/

Here's an example of me doing some serious goofing with a few of these commands (whatever you do, don't use sudo 🔫): 

![image](https://maximpodgore.github.io/cse15l-lab-reports/img7.png)  



