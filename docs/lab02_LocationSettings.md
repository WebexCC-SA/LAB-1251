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



# Lab 2 - Location Settings

In this lab, you will learn how to add locations.

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
<td><p id="p1">Management-&gt; Locations-&gt; dCloud-&gt; Location info</p></td>
</tr>
<tr>
<td><p id="p2">San Jose is the headquarters and main location</p>
<p>Rename dCloud location</p>
<ul>
<li><p>Location name: HQ</p></li>
</ul></td>
</tr>


<tr>
<td rowspan="2"><p id="p1">2.</p></td>
<td><p id="p1">Management-&gt; Locations-&gt; Manage locations-&gt; Create
manually</p></td>
</tr>
<tr>
<td><p id="p2">Paw Pet Solutions has a factory in Houston, TX.</p>
<p>Add a location</p>
<ul>
<li><p>Location name: Factory</p></li>
<li><p>Address: 4501 North Main Street, Houston, TX 77009, USA</p></li>
<li><p>Time zone: Chicago</p></li>
<li><p>Country – USA</p></li>
<li><p>Language – English</p></li>
<li><p>Click “Set up calling” after creating your location and then
close the PSTN connection window.You will set up the PSTN connection in another step</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2"><p id="p1">3.</p></td>
<td><p id="p1">Management-&gt; Locations-&gt; Select location-&gt; Calling-&gt;
PSTN connection</p></td>
</tr>
<tr>
<td><p id="p2">HQ and Factory will use the Cisco Calling Plan</p>
<p>Assign a PSTN Connection to each location</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Connection Type: Cisco Calling Plans</p></li>
<li><p>Contract Information: Your name, Student login email
address</p></li>
<li><p>Services Address: HQ location address (already entered)</p></li>
<li><p>Authorized Contact: Your name</p></li>
<li><p>Job title: Admin</p></li>
</ul>
<p>Repeat steps for Factory location</p>
</td>

</tr>
<tr>
<td rowspan="2"><p id="p1">4.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Numbers-&gt; Manage-&gt; Add</p></td>
</tr>
<tr>
<td><p id="p2">Each location needs 10 numbers</p>
<p>Add Numbers</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Number Type: PSTN</p></li>
<li><p>Select an Area Code from the list</p></li>
<li><p>Select 10 numbers</p></li>
<li><p>Click view orders</p></li>
<li><p>Click on the pending order to automatically change the status to
provisioned</p></li>
</ul>
<p>Repeat steps for Factory location</p>
</td>
</tr>
<tr>
<td rowspan="2"><p id="p1">5.</p></td>
<td><p id="p1">Management-&gt; Locations-&gt; Select location -&gt; Calling-&gt;
Calling Connection-&gt; Main number</p></td>
</tr>
<tr>
<td><p id="p2">To make and receive calls each location needs a main number. Each
location must present their own main number as their caller id.</p>
<p>Assign a main number to each location</p>
<ul>
<li><p>Select any of the available numbers</p></li>

</ul>
<p>You will need to know your locations main number in a subsequent lab; make a
note of which ones you use.</p>
</td>
</tr>
<tr>
<td rowspan="2"><p id="p1">6.</p></td>
<td><p id="p1">Management-&gt; Locations-&gt; Select location -&gt; Calling-&gt;
Dialing-&gt; Internal dialing</p></td>
</tr>
<tr>
<td><p id="p2">All location extensions are mirror images of each other.</p>
<p>Add a routing prefix for each location</p>
<ul>
<li><p>HQ: 81</p></li>
<li><p>Factory: 82</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2"><p id="p1">7.</p></td>
<td><p id="p1">Management-&gt; Locations-&gt; Select location -&gt; Calling-&gt;
Calling features settings-&gt; Voice portal</p></td>
</tr>
<tr>
<td><p id="p2">All locations need voicemail.</p>
<p>Configure the voice portal for each location</p>
<ul>
<li><p>Incoming Call:Extension 200</p></li>
<li><p>Voice Portal Admin Passcode: 137041</p></li>
<li><p>Language: English</p></li>
</ul>
<p>Repeat steps for Factory location</p>
</td>
</tr>
<tr>
<td rowspan="2"><p id="p1">8.</p></td>
<td><p id="p1">Management-&gt; Locations-&gt; Select location -&gt; Calling-&gt;
Calling features settings-&gt; Schedules</p></td>
</tr>
<tr>
<td><p id="p2">Calls coming into the main numbers need to route to specific
options based on the time of day.</p>
<p>Create a schedule for HQ and Factory locations</p>
<ul>
<li><p>Name: Open Hours</p></li>
<li><p>Schedule Type: Business Hours</p></li>
<li><p>Monday – Friday 9:00 am – 5 pm</p></li>
</ul>
</td>
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