<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
Part 3 of a three-part osTicket Install/Configuration/Ticket-Creation tutorial series. This final section outlines the lifecycle of a ticket from intake to resolution using osTicket.<br/>

<h2>Environments and Technologies Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machines/Compute)</li>
  <li>Remote Desktop</li>
  <li>Internet Information Services (IIS)</li>
</ul>

<h2>Operating Systems Used</h2>
<ul>
  <li>Windows 10 (21H2)</li>
</ul>

<h2>Admin and User Access URLs</h2>
<ul>
  <li><strong>Admin/Analyst Login Page:</strong> <a href="http://localhost/osTicket/scp/login.php">http://localhost/osTicket/scp/login.php</a></li>
  <li><strong>End Users osTicket URL:</strong> <a href="http://localhost/osTicket">http://localhost/osTicket</a></li>
</ul>

<h2>Lab Objectives</h2>
<ul>
  <li>Create and manage tickets as both end users and agents</li>
  <li>Practice setting SLA, priority, and departmental routing</li>
  <li>Understand permissions and escalation workflows</li>
</ul>

<h2>Initial Setup</h2>
<ul>
  <li>Change the <strong>SysAdmins</strong> department to a Top Level Department</li>
  <li>Delete the <strong>Maintenance</strong> department (do not archive)</li>
</ul>

<h2>Ticket Scenario 1</h2>

<h3>Stage 1: Intake</h3>
<p><strong>End-User Action:</strong> Create a ticket with the following:</p>
<ul>
  <li>Help Topic Dropdown Menu: Business Critical Outage</li>
<ul><li>- Issue Summary: Entire mobile online banking is down</li>
  <li>- Details: Customers are reporting they are getting a 404 error when browsing to online banking.</li></ul>
    <li><strong>Issue:</strong> Entire mobile/online banking system is down
  </li>
  <li>Email Address: me.marcusdunlap@tech</li>
  <li>Name: Marcus Dunlap</li>
</ul>

<h3>Stage 2: Assignment and Communication</h3>
<p><strong>Agent: John</strong></p>
<ul>
  <li>Review ticket properties (Priority, SLA, Department, Assigned To)</li>
  <li>Set SLA to <strong>SEV-A (1 hour, 24/7)</strong></li>
  <li>Set Department to <strong>Online Banking Department</strong></li>
  <li>Re-attempt to view ticket — access should now be restricted</li>
</ul>

<p><strong>Agent: Jane</strong></p>
<ul>
  <li>Work the ticket and provide resolution as Jane</li>
</ul>

<p align="center">
  <img src="https://i.imgur.com/DJmEXEB.png" height="70%" width="70%" alt="Ticket Example 1"/>
</p>

<h2>Ticket Scenario 2</h2>

<h3>Stage 1: Intake</h3>
<p><strong>End-User Action:</strong> Create a ticket with the following:</p>
<ul>
  <li><strong>Issue:</strong> Accounting department needs Adobe upgrade, broken</li>
</ul>

<h3>Stage 2: Assignment and Communication</h3>
<p><strong>Agent: John</strong></p>
<ul>
  <li>Review ticket properties</li>
  <li>Set SLA to <strong>SEV-B (4 hours, 24/7)</strong></li>
  <li>Assign to <strong>Support</strong> department</li>
  <li>Work the ticket to completion as John</li>
</ul>

<p align="center">
  <img src="https://i.imgur.com/DJmEXEB.png" height="70%" width="70%" alt="Ticket Example 2"/>
</p>

<h2>Ticket Scenario 3</h2>

<h3>Stage 1: Intake</h3>
<p><strong>End-User Action:</strong> Create a ticket with the following:</p>
<ul>
  <li><strong>Issue:</strong> CFO’s laptop will no longer turn on</li>
</ul>

<h3>Stage 2: Assignment and Communication</h3>
<p><strong>Agent: John</strong></p>
<ul>
  <li>Review ticket properties</li>
  <li>Set SLA to <strong>SEV-B (4 hours, 24/7)</strong></li>
  <li>Assign to <strong>Support</strong> department</li>
  <li>Work the ticket to completion as Jane</li>
</ul>

<p align="center">
  <img src="https://i.imgur.com/DJmEXEB.png" height="70%" width="70%" alt="Ticket Example 3"/>
</p>

<h2>Escalation and Permissions</h2>
<ul>
  <li>Change all tickets’ SLA to <strong>SEV-A</strong></li>
  <li>Observe that tickets routed to <strong>SysAdmins</strong> become inaccessible to john</li>
  <li>Log in as Admin and grant view-access to john for the <strong>SysAdmins</strong> department</li>
  <li>Return to agent panel; note ticket is now viewable but not editable</li>
</ul>

<h2>Finalizing and Closing Tickets</h2>
<ul>
  <li>Resolve each ticket and ensure their statuses are set to <strong>Closed</strong></li>
  <li>osTicket supports email communication — updates and replies can be sent and received automatically</li>
</ul>

<h2>Real-World Ticket Intake</h2>
<p>Tickets in real-world scenarios can originate from:</p>
<ul>
  <li>Phone calls</li>
  <li>Chat apps</li>
  <li>Emails</li>
  <li>Web forms</li>
  <li>In-person conversations</li>
</ul>
<p>Always document support actions in a ticket, even if handled on the spot. This builds metrics and accountability.</p>

<h2>Practice and Mastery</h2>
<ul>
  <li>Explore osTicket's features like automation, canned responses, and ticket filters</li>
  <li>Repeat this lab until the process is intuitive</li>
</ul>

<h2>Technical Skill Pillar</h2>
<p>Hands-on practice with osTicket helps reinforce core technical support skills including system navigation, documentation, ticket routing, and resolution procedures.</p>

<p><strong>🎉 Congratulations! You have completed the final part of the osTicket series. 🎉</strong></p>
