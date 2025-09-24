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


# Lab 5 - Workspaces

In this lab, you will learn how to create workspaces, assign devices to workspaces, and enable hoteling and hotdesking on workspace devices.

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
<col style="width: 6%" />
<col style="width: 93%" />
</colgroup>
<tbody>
<tr>
<td rowspan="2"><p id="p1">1.</p></td>
<td><p id="p1">Management-&gt; Workspaces-&gt; Add Workspace</p></td>
</tr>
<tr>
<td><p id="p2">Paw Pet Supply Solutions has 4 shared use areas in which they need to hold meetings and make and receive calls</p>
<p>Add the workspaces with the corresponding devices and services. Devices will be added using activation code.</p>
</td>
</tr>
<tr>
<td colspan="2"><table>
<colgroup>
<col style="width: 18%" />
<col style="width: 10%" />
<col style="width: 13%" />
<col style="width: 16%" />
<col style="width: 30%" />
<col style="width: 10%" />
</colgroup>
<tdead>
<tr>
<td>Workspace name</td>
<td>Type</td>
<td>Location</td>
<td>Device</td>
<td>Services</td>
<td>Extension</td>
</tr>
</tdead>
<tbody>
<tr>
<td>SharedCubicle1</td>
<td>Desk</td>
<td>HQ</td>
<td>Cisco Managed Device: Cisco 8865</td>
<td><p>Cisco Webex Calling</p>
<p>Common area workspace</p></td>
<td>201</td>
</tr>
<tr>
<td>SharedCubicle2</td>
<td>Desk</td>
<td>HQ</td>
<td>Cisco Managed Device: Cisco 8865</td>
<td><p>Cisco Webex Calling</p>
<p>Common area workspace</p></td>
<td>202</td>
</tr>

<tr>
<td>Conference Room1</td>
<td>Meeting Room</td>
<td>HQ</td>
<td>Cisco Room and Desk device</td>
<td>Cisco Webex Calling Professional workspace</td>
<td>300</td>
</tr>

<tr>
</tr>
<tr>
<td>Conference Room2</td>
<td>Meeting Room</td>
<td>Factory</td>
<td>Cisco Room and Desk device</td>
<td>Cisco Webex Calling Professional workspace</td>
<td>300</td>
</tr>
<tr>
</tr>
</tbody>
</table></td>
</tr>
<tr>
<td rowspan="2"><p id="p1">2.</p></td>
<td><p id="p1">Management-&gt; Workspaces-&gt; SharedCubicle1-&gt;
Scheduling</p></td>
</tr>
<tr>
<td><p id="p2">To conduct calls in private, users may sometimes need to access
all of their configured lines from a location other than their usual
desk.</p>
<p>Verify that Hot Desk Sign in is selected</p>
</td>
</tr>

<tr>
<td rowspan="2"><p id="p1">3.</p></td>
<td><p id="p1">Management-&gt; Workspaces-&gt; SharedCubicle2-&gt;
Scheduling</p></td>
</tr>
<tr>
<td><p id="p2">To enable hoteling, its needed to disable hot desking for the Workspace.</p>
<p>Disable Hot Desk Sign in </p>
</td>
</tr>



<tr>
<td rowspan="2"><p id="p1">4.</p></td>
<td><p id="p1">Management-&gt; Devices-&gt; SharedCubicle2&gt; Hoteling</p></td>
</tr>
<tr>
<td><p id="p2">To conduct calls in private, users may sometimes need to make and
receive calls in a space other than their typical desk. Most of these
users only have a primary line.</p>
<p>Enable device to be used as a hoteling host</p>
<ul>
<li><p>Device: Cisco 8865 belonging to SharedCubicle2</p></li>
<li><p>Hoteling: Enable</p></li>
<li><p>Limit the time a guest can use this phone to 12 hours</p></li>
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