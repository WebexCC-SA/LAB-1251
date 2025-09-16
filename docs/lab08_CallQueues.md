<style>

  td  {
    font-style: normal;
    font-size: 16px;
    }


    #p1 {
    color: #00B050;
    font-weight: bold;
    }

  #p2 {
    color: #4BACC6;
    font-weight: bold;
    }

  #p3 {
    font-weight: bold;
    }
    
  #p4 {
    color: red;
    font-weight: bold;
    text-align: center;
    font-size: 30px;
    }

  .container {
  text-align: center;
  }

</style>


# Lab 8 - Creating Call Queues

In this lab, you will learn how to create call queues.

## Login Credentials

<table>
<tr>
<td><p id="p3">URL</p></td>
<td><a href="https://admin.webex.com">admin.webex.com</a></td>
</tr>
<tr>
<td><p id="p3">Login</p></td>
<td>Charles Holland – Webex Administrator </td>
</tr>
</table>

## Instructions

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<tbody>
<tr>
<td rowspan="2"><p id="p1">1.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Features-&gt; Call Queue-&gt; Add New</p></td>
</tr>
<tr>
<td><p id="p2">During business hours, callers to the San Jose Support and Sales departments should be placed on hold until an agent is available.</p>
<p>Create a Call Queue</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Name: Sales Queue</p></li>
<li><p>Phone Number: HQ Main Number (taken from Lab02)</p></li>
<li><p>Extension: 900</p></li>
<li><p>Number of calls in queue: 15</p></li>
<li><p>External caller ID phone number: Location number</p></li>
<li><p>Routing: Priority Based - Longest Idle</p></li>
<li><p>Overflow Settings: </p>
<ul>
<li><p>Transfer to phone number: Anita Perez Ext 81-101</p></li>
<li><p>Enable over flow after 60 seconds</p></li>
</ul>
</li>

<li><p>Welcome Message:</p>
<ul>
<li><p>Welcome Message is mandatory: Enabled</p></li>
<li><p>Custom Welcome Message: All-Calls-are-Recorded.wav</p></li>
</ul></li>


<li><p>Comfort Message: Enabled</p>
<ul>
<li><p>Time between comfort message: 10 seconds</p></li>
<li><p>Custom Comfort Message: Default Greeting</p></li>
</ul></li>

<li><p>Hold Music: Enabled</p>
<ul>
<li><p>Hold Music: Play default music</p></li>
</ul>
</li>

<li><p>Agents:</p>
<ul>
<li><p>Sales1@YourFullName##.com</p></li>
<li><p>Sales2@YourFullName##.com</p></li>
<li><p>Eric Steele</p></li>
<li><p>Kellie Melby</p></li>
</ul></li>

<li><p>Create Queue</p></li>
<li><p>Select Queue</p></li>
<li><p>Go to Queue Policies, select Night Service</p>
<ul>
<li><p>Enable Night Service:</p></li>
<li><p>Transfer to Phone number: Extension 81-600 (VmailGroup)</p></li>
<li><p>Default Greeting</p></li>
<li><p>Business Hours: Open Hours schedule</p></li>
</ul>
</li>
<li><p>Go to Queue Policies, select Stranded Calls</p>
<ul>
<li><p>Triger policy when all agents are unreachable: enabled</p></li>
<li><p>Night Service: selected</p></li>
</ul>
</li>

</ul></td>
</tr>


<tr>
<td rowspan="2"><p id="p1">2.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Features-&gt; Call queue-&gt;Supervisors-&gt; Add Supervisor</p></td>
</tr>
<tr>
<td><p id="p2">The supervisor needs to silently monitor agents in their respective queues</p>
<ul>
<li><p>Supervisor: Charles Holland</p></li>
<li><p>Agents:</p>
<ul>
<li><p>Sales1@YourFullName##.com</p></li>
<li><p>Sales2@YourFullName##.com</p></li>
<li><p>Eric Steele</p></li>
<li><p>Kellie Melby</p></li>
</ul></li>
</ul></td>
</tr>
</tbody>
</table>

<p id="p4">STOP - END OF LAB</p>

<div class="container">
<svg xmlns="http://www.w3.org/2000/svg" width="200" height="200" fill="red" class="bi bi-sign-stop-fill" viewBox="0 0 16 16">
  <path d="M10.371 8.277v-.553c0-.827-.422-1.234-.987-1.234-.572 0-.99.407-.99 1.234v.553c0 .83.418 1.237.99 1.237.565 0 .987-.408.987-1.237m2.586-.24c.463 0 .735-.272.735-.744s-.272-.741-.735-.741h-.774v1.485z"/>
  <path d="M4.893 0a.5.5 0 0 0-.353.146L.146 4.54A.5.5 0 0 0 0 4.893v6.214a.5.5 0 0 0 .146.353l4.394 4.394a.5.5 0 0 0 .353.146h6.214a.5.5 0 0 0 .353-.146l4.394-4.394a.5.5 0 0 0 .146-.353V4.893a.5.5 0 0 0-.146-.353L11.46.146A.5.5 0 0 0 11.107 0zM3.16 10.08c-.931 0-1.447-.493-1.494-1.132h.653c.065.346.396.583.891.583.524 0 .83-.246.83-.62 0-.303-.203-.467-.637-.572l-.656-.164c-.61-.147-.978-.51-.978-1.078 0-.706.597-1.184 1.444-1.184.853 0 1.386.475 1.436 1.087h-.645c-.064-.32-.352-.542-.797-.542-.472 0-.77.246-.77.6 0 .261.196.437.553.522l.654.161c.673.164 1.06.487 1.06 1.11 0 .736-.574 1.228-1.544 1.228Zm3.427-3.51V10h-.665V6.57H4.753V6h3.006v.568H6.587Zm4.458 1.16v.544c0 1.131-.636 1.805-1.661 1.805-1.026 0-1.664-.674-1.664-1.805V7.73c0-1.136.638-1.807 1.664-1.807s1.66.674 1.66 1.807ZM11.52 6h1.535c.82 0 1.316.55 1.316 1.292 0 .747-.501 1.289-1.321 1.289h-.865V10h-.665V6.001Z"/>
</svg>
</div>