<h1>Creating a New Group Policy (Disabling Task Manager)</h1>


<h2>Description</h2>
<p>In this section, I will create a new group policy that will apply to John, who works in the HR department. The new group policy will restrict John from using the "Task Manager".</p>


<br />

<h2>Step-by-Step Walk-Through:</h2>


<p align="center"> 
STEP 1: <br/>
<img src="https://i.imgur.com/NVLwotz.png" height="70%" width="70%"/> </p>


<p align="center">The first step is to open Server Manager on the Server device. I then select the "TOOLS" option, which is placed in the top right corner of the screen. This will provide me additional options in the Server Manager.</p>


<hr width="100%" size="2">

<br />

<p align="center"> 
STEP 2: <br/>
<img src="https://i.imgur.com/wwBvgzt.png" height="40%" width="40%"/> </p>


<p align="center">I navigate to the "Tools" area and then select "GROUP POLICY MANAGEMENT". This allows me to view the "Group Policy" section of the domain "office123.com".</p>


<hr width="100%" size="2">

<br />

<p align="center"> 
STEP 3: <br/>
<img src="https://i.imgur.com/80IcRWk.png" height="80%" width="80%"/> </p>


<p align="center">This is the Group Policy Management section, and from here I locate the "Group Policy Objects" folder. I then right-click on that folder and choose "NEW" to create a new group policy for the domain.</p>


<br />
<br />

<p align="center"> 
<img src="https://i.imgur.com/OSfgEvT.png" height="70%" width="70%"/> </p>


<p align="center">I'm typing a name for the new group policy. In this situation, I named the policy "Disable Task Manager" to better represent the actual policy and make it easier to identify. I then move on to the next step.</p>


<hr width="100%" size="2">

<br />

<p align="center"> 
STEP 4: <br/>
<img src="https://i.imgur.com/z2Zl5yJ.png" height="70%" width="70%"/> </p>


<p align="center">As you can see, a new group policy object has been created with the name "Disable Task Manager". Now I need to add John to this policy to ensure that he does not have access to the Task Manager program. To do so, I need to first click on the group policy object and then navigate to the "Delegation" section. I then added John's account from there, giving him restricted "READ" permissions for security purposes. Now I move on to the next step.</p>


<hr width="100%" size="2">

<br />

<p align="center"> 
STEP 5: <br/>
<img src="https://i.imgur.com/2yaRa5U.png" height="70%" width="70%"/> </p>


<p align="center">Here, I right-click on the group policy object and select "EDIT". This section will let me disable the "Task Manager" application.</p>


<hr width="100%" size="2">

<br />

<p align="center"> 
STEP 6: <br/>
<img src="https://i.imgur.com/kEmCXDh.png" height="70%" width="70%"/> </p>


<p align="center">This is the "group policy editor" section for the new group policy object that I just created. From here, I locate and open the "CTRL+ALT+DEL Options" folder. By entering this folder, I will be able to turn off the Task Manager application. I then double-click on the "REMOVE TASK MANAGER" option to reveal additional options.</p>

<br />
<br />

<p align="center"> 
<img src="https://i.imgur.com/idmBY0G.png" height="60%" width="60%"/> </p>


<p align="center">Here, I enable the option that allows me to disable the Task Manager application. I then click "Apply" to save the changes.</p>


<br />
<br />

<p align="center"> 
<img src="https://i.imgur.com/3QLwLio.png" height="60%" width="60%"/> </p>

<p align="center">I've moved the group policy object to the HR folder. This will apply the new group policy object to the HR department where John is located.</p>


<hr width="100%" size="2">

<br />

<p align="center"> 
STEP 7: <br/>
<img src="https://i.imgur.com/gilw3UZ.png" height="70%" width="70%"/> </p>


<p align="center">Now I'm on John's PC to update the group policy settings for his account. To do that, I need to open the Command Prompt and type "GPUPDATE /FORCE". This will successfully update the group policy settings under John's account.</p>

<br />
<br />

<p align="center"> 
<img src="https://i.imgur.com/ecd9mfg.png" height="90%" width="90%"/> </p>

<p align="center">I'm still in the Command Prompt, and I type the command "GPRESULT /R" to see if the new group policy object was successfully updated to John's PC. As you can see, the group policy "DISABLE TASK MANAGER" has been successfully applied and will take effect immediately.</p>


<br />
<br />

<p align="center"> 
<img src="https://i.imgur.com/eNaJAzx.png" height="70%" width="70%"/> </p>

<p align="center">Here, I use the keyboard shortcut "CTRL+ALT+DEL" to see if the Task Manager program exists on John's computer. As you can see, the Task Manager is not available and John cannot access it.</p>



<a href="https://www.example.com">
  <button>NEXT</button>
</a>
