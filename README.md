<h1>Virtual machine Scale set</h1>

<h2>Description</h2>
This lab will create a Virtual machine scale set.<br />
This lab will be create a virtual machine scale set using a Linux server. Stress will be induced on the Linux server and the scale set will automatically scale up. When the stress is removed the scale set will automatically scale down.<br />


<h2>Environments Used </h2>

- <b>Microsoft Azure</b>

<h2>Lab walk-through:</h2>

<p align="center">
<h4>Step 1</h4>
Create a Vitual machine Scale Set resource<br/>
<img src="https://i.imgur.com/16okTqS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
If you go to instances you will see that there is only one instance of the VM running..<br/>
<img src="https://i.imgur.com/0rnPu3T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
<br />

<h4>Step 2</h4> 
Go to scaling --> Custom auto-scale and Rues for scaling up and down.<br/>
<img src="https://i.imgur.com/FuUX7IF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
<br />

<h4>Step 3</h4>
<br />
Before stress is induced the CPU usage is <20%<br/>
<img src="https://i.imgur.com/CtIhJax.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
<br />
Log into your Linux machine and induce stress on the CPU<br/>
<img src="https://i.imgur.com/4cC9Z13.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>


<h4>Step 4</h4> 
After 10 mins the CPU usage is >70%.<br/>
<img src="https://i.imgur.com/snliwB2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
<br />
The instances have been scaled from 1 to 2.<br/>
<img src="https://i.imgur.com/dA0zErZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>

<h4>Step 5</h4> 
On the Linux machine, remove the stress on the CPU.<br/>
<img src="https://i.imgur.com/tainOKF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>
<br />
After 10 minutes the instnces will be scaled down, from 2 t 1.<br/>
<img src="https://i.imgur.com/FjCbPaR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br/>


