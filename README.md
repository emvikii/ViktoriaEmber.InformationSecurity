This is where I do the homeworks for Information Security course.

<!DOCTYPE html>
<html>
    <head>
        Homeworks
    </head>
   <br>
    <br>
Homework 1
    </body>
<h3>
x) Read and summarize. Hutchins et al 2011: Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains, chapters Abstract, 3.2 Intrusion Kill Chain and 3.3 Courses of Action
</h3>
<h4> Abstract <h/4>

- Traditional incident response methodologies assume an intrusion that is successful, while traditional network defense products like intrusion detection systems and anti-virus concentrate on the vulnerability component of risk.

 - These strategies are no longer adequate for some players due to the growth of the objectives and expertise of computer network attacks. The term "Advanced Persistent Threat" (APT) refers to a new category of threats that are well-resourced and skilled adversaries who run multi-year infiltration campaigns against extremely sensitive commercial, proprietary, or national security information.

<h4> 3 Intelligence-driven Computer Network Defense </h4>

- A risk management method that tackles the threat element of risk by analyzing opponents' capabilities, aims, ideology, and limits is known as intelligence-driven computer network defense. This must be an ongoing process that uses indicators to find new activities that may be supported by more indicators. It necessitates a fresh perspective on the incursions themselves, one that views them as gradual progressions rather than as isolated incidents. In order to analyze intrusions and guide a defensive course of action, this study introduces a new intrusion kill chain model.

- An intelligence-driven CND has the effect of strengthening the security posture. APT actors try infiltration after an incursion by nature, modifying their activities based on each attempt's success or failure. Any repeat by the attacker is a disadvantage that defenders must notice and exploit since in a kill chain model, only one mitigation breaks the chain and thwarts the adversary.

<h4> 3.1 Indicators and the Indicator Life Cycle </h4>
 
The indicator is the primary component of intelligence in this approach. Three categories of indicators exist:
    
- atomic
- computed
- behavioural


<h4> 3.2 Intrusion Kill Chain </h4>
A kill chain is a systematic way to confront an enemy and produce the desired results. This integrated, end-to-end process is called a "chain" because any one link could break.
 
-	Reconnaissance
-	Weaponization
-	Delivery
-	Exploitation
-	Installation
-	Command and Control (C2)
-	Actions on Objectives

<h4> 3.4 Intrusion Reconstruction </h4>

- An analyst can use kill chain analysis as a guide to identifying what data is and might be accessible for the protective course of action. It's a model for conducting fresh analysis of the invasions.
- Most intrusions that are discovered only offer a small number of characteristics regarding one particular stage of the intrusion. To enumerate the most possible possibilities for courses of action, analysts must still identify numerous additional characteristics for each step.
- Furthermore, analysts can infer that earlier stages of the intrusion have already been successfully completed based on detection in a particular phase.

<br>
</br>
 
<h2> A summary of Karvinen 2020: Command Line Basics Revisited </h2>
    
<h4> Moving and looking around </h4>
    
 $ pwd - 
'pwd' prints the working directory.


$ ls - 
List files in working directory. These are the files you can directly manipulate.

$ cd terosdir/ - 
Change directory to "terosdir", under working directory.

$ cd .. - 
Change directory up. Path printed by pwd becomes shorter. Note space between command "cd" and directory "..".

$ less tero.txt - 
View text file tero.txt. In 'less', space " " shows next page, "b" shows previous page, slash "/" searches, "q" exits

$ ls /etc|less - 
Any command output can be read one screenfull at a time by piping the output to less. On Finnish keyboard, pipe character is created by pressing AltGr (right of space) and “<>|” (between left shift and Z)

<h4> File Manipulation </h4>
Easiest text editors are pico and nano.

$ nano FOO.TXT
Use CTRL-X y Enter to save and exit. You can see all commands at the bottom of nano screen. There the hat character “^” means control, for example “^X” is the same as ctrl-X.

Filenames don’t have to be ALL CAPS, capitalization is used just for readability. If FOO.TXT does not exist, it is created. Files can have any suffix, and text file names don’t often end with “.txt”.

Make a new directory (ie. folder):

$ mkdir NEWFOLDER
Move or rename directory or file OLDNAME to target NEWNAME. If NEWNAME does not exist, OLDNAME is renamed to NEWNAME.

$ mv OLDNAME NEWNAME
If both parameters are files, NEWNAME is overwritten. Usually no warnings or questions are shown.

If target is a directory, OLDNAME is moved there.

$ mv SOMEFILE NEWDIR/
Copy ORIGINAL to COPY. “-r” means recursive, ORIGINAL is copied with contents if it is a directory.

$ cp -r ORIGINAL COPY
Remove an empty directory

$ rmdir EMPTYDIR
Remove a file called JUNK.

$ rm JUNK
Remove FOLDEROFJUNK/ and its contents. Usually no warnings or questions are shown.

$ rm -r FOLDEROFJUNK
There is no trash with rm. Think before you type.

<h4>SSH Remote Control </h4>
Open a remote command shell in a very secure way. Here, username is tero and server is example.com.

$ ssh tero@example.com
A command line just like yours opens. 

Exit back to your own machine with ‘exit’

remotecomputer$ exit
Securely copy FOLDER to a folder in remote machine. Scp is run on your own machine. If you are connected to remote computer with ssh, ‘exit’ first.

$ scp -r FOLDER tero@example.com:public_html/

</html>
