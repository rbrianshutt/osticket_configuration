<h1>osTicket Configuration</h1>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/osticket-logo1.png)


<h2>Description</h2>
Lorem ipsum
<br />

<h2>Techonologies Used</h2>

- <b>Microsoft Azure</b> 
- <b>Remote Desktop</b>
- <b>OsTicket</b>
- <b></b>
- <b></b>

<h2>Operating Systems</h2>

- <b>Windows 10 </b> 

<h2>Dependencies</h2>

- <b>PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)</b> 
- <b>Rewrite Module (rewrite_amd64_en-US.msi)</b>
- <b>PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip)</b> 
- <b>VC_redist.x86.exe</b>
- <b>MySQL 5.5.62 (mysql-5.5.62-win32.msi)</b> 
- <b>HeidiSQL</b>

<h2>Program walk-through:</h2>

<h3>Set up virtual environment</h3>
Create an Azure Virtual Machine  <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/1.Create%20an%20Azure%20Virtual%20Machine.PNG)
<br />
<br />
Log into the VM with Remote Desktop <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/2.Log%20into%20the%20VM%20with%20Remote%20Desktop.PNG)
<br />
<br />
<h3>Login Pages</h3>
Admin/Analyst Login Page: <br/>
http://localhost/osTicket/scp/login.php  <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/3%20osTicket%20login.PNG)
<br />
<br />
End Users osTicket URL:<br/>
http://localhost/osTicket <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/3.1.support%20center.PNG)
<br />
<br />
Admin Panel <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/4.admin%20panel.PNG)
<br />
<br />
Agent Panel <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/4.agent%20panel.PNG)
<br />
<br />

<h3>Configure Roles (for grouping permissions)</h3>
Admin Panel -> Agents -> Roles<br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/5.1%20congfigure%20role1.PNG)
<br />
<br />
Name role Supreme Admin <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/5.2configure%20role.PNG)
<br />
<br />
Add ticket permissions <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/5.3add%20permissions%20tickets.PNG)
<br />
<br />
Add task permissions  <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/5.4add%20permissions%20tasks.PNG)
<br />
<br />
Add knowledge base permissions  <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/5.5%20add%20permissions%20knowledgebase.PNG)
![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/5.6%20added%20supreme%20admin.PNG)
<br />
<br />
<h3>Configure Departments</h3>
Admin Panel -> Agents -> Departments <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/6.1add%20department.PNG)
<br />
<br />
Name department SysAdmins  <br/>
Parent set to Top Level Department  <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/6.2%20create%20sysadmins.PNG)
![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/6.3created.PNG)
<br />
<br />
<h3>Configure Teams</h3>
Admin Panel -> Agents -> Teams (Pull Agents from different Departments)  <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/7.1add%20new%20team.PNG)
<br />
<br />
Name new team: Online Banking  <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/7.2online%20banking%20team.PNG)
![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/7.3%20team%20added.PNG)
<br />
<br />
<h3>Allow anyone to create tickets</h3>
Admin Panel -> Settings -> User Settings (UNCHECK: Registration Required: Require registration and login to create tickets)  <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/8.1uncheck%20unregistered%20users%20can%20create%20tickets.PNG)
<br />
<br />
<h3>Configure Agents (workers)</h3>
Admin Panel -> Agents -> Add New <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/9.1add%20new%20agent.PNG)
<br />
<br />
Agent Jane Doe - Add name, email, and username  <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/9.2janedoe.PNG)
<br />
<br />
Assign access to primary departments : SysAdmins <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/9.3access.PNG)
<br />
<br />
Assign permissions <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/9.4permissions.PNG)
<br />
<br />
Assign the agent a team: Online Banking  <br/>
Click create
![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/9.5teams.PNG)
![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/9.6jane%20doe%20added.PNG)
<br />
<br />
Add agent John Doe - Add name, email, and username <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/9.7add%20agent%20john%20doe.PNG)
<br />
<br />
Assign access to primary departments : Support  <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/9.8%20access.PNG)
<br />
<br />
Assign permissions <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/9.9persmissions.PNG)
<br />
<br />
Assign a team if need  <br/>
Click create <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/9.10agents.PNG)
![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/9.11agent%20added.PNG)
<br />
<br />
<h3>Configure Users (customers)</h3>
Agent Panel -> Users -> Add New <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/10.1add%20user.PNG)
<br />
<br />
Enter user name Karen and email address  <br/>
Click Add user  <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/10.2karen.PNG)
![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/10.3user%20added.PNG)
<br />
<br />
<h3>Configure SLA</h3>
Admin Panel -> Manage -> SLA  <br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/11.1add%20sla.PNG)
<br />
<br />
Enter name: Severity A  <br/>
Grace period: 1 hr<br/>
Schedule: 24/7<br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/11.2severity%20a.PNG)
<br />
<br />
Enter name: Severity B  <br/>
Grace period: 4 hr<br/>
Schedule: 24/7<br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/11.3severity%20b.PNG)
<br />
<br />
Enter name: Severity C  <br/>
Grace period: 8 hr<br/>
Schedule: Business Hours<br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/11.4severity%20c.PNG)
![](hub.com/rbrianshutt/osticket/blob/main/osTicket/11.5severity%20added.PNG)
<br />
<br />
<h3>Configure Help Topics (For when users create a ticket)</h3>
Admin Panel -> Manage -> Help Topics<br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/12.1add%20new%20help%20topic.PNG)
<br />
<br />
Enter topic: Business Critical Outage <br/>
Parent topic: Report a problem<br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/12.2business%20critical%20outage.PNG)
![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/12.3business%20critical%20added.PNG)
<br />
<br />
Enter topic: Personal Computer Issues<br/>
Parent topic: Report a problem<br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/12.4personal%20computer%20issues.PNG)
<br />
<br />
Enter topic: Equipment Request<br/>
Parent topic: General Inquiry<br/>


![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/12.5equipment%20request.PNG)
<br />
<br />
Enter topic: Password Reset<br/>
Parent topic: Report a problem<br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/12.6password%20reset.PNG)
<br />
<br />
Enter topic: Other<br/>
Parent topic: General Inquiry<br/>

![](https://github.com/rbrianshutt/osticket/blob/main/osTicket/12.7other.PNG)
<br />
<br />
Lorem ipsum  <br/>

![]()
<br />
<br />
Lorem ipsum  <br/>

![]()
<br />
<br />
Lorem ipsum  <br/>

![]()
<br />
<br />
Lorem ipsum  <br/>

![]()
<br />
<br />
Lorem ipsum  <br/>

![]()
<br />
<br />
Lorem ipsum  <br/>

![]()
<br />
<br />
Lorem ipsum  <br/>

![]()
<br />
<br />
