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


# Lab 7 - Configuring Calling features

In this lab, you will learn how to create virtual extensions, call park extensions, and call park groups.

- Paw Pet Supply Solutions desire their telephone system configured in a certain way: 

    * Call Park Group configured with call park extensions
    * Call Pickup
    * A way to bring anouncements with a Paging Group
    * After Hours Voicemail Group
    * A way for Rebekah to route the calls to the Product Development department to voicemail at will
    * Marketing and Product Development departments need their own extension
    * Factory main number routed to an IVR

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
<td><p id="p1">Services-&gt; Calling-&gt; Features-&gt; Call park extension-&gt;
Add New</p></td>
</tr>
<tr>
<td><p id="p2">The sales department needs to place callers on hold for team members to pick them up from any device without tying up their personal extensions.</p>
<p>Create call park extensions</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Names &amp; Extensions:</p>
<ul>
<li><p>Extension 1 – 401</p></li>
<li><p>Extension 2 – 402</p></li>
<li><p>Extension 3 – 403</p></li>
</ul></li>
</ul></td>
</tr>


<tr>
<td rowspan="2"><p id="p1">2.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Features-&gt; Call park group-&gt; Add New</p></td>
</tr>
<tr>
<td><p id="p2">Create a call park group</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Name: Sales CP Group</p></li>
<li><p>Members:</p>
<ul>
<li><p>Kellie Melby</p></li>
<li><p>Sales1@YourFullName##.com</p></li>
<li><p>Sales2@YourFullName##.com</p></li>
</ul></li>
<li><p>Park Destinations: Call Park Extensions 401, 402, 403</p>
<ul>
<li><p>Recall: Alert Parking User Only</p></li>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2"><p id="p1">3.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Features-&gt; Call pickup-&gt; Add New</p></td>
</tr>
<tr>
<td><p id="p2">the Sales Department employees need to answer each other calls
when other team members in the same location are unavailable.</p>
<p>Create Pickup Group</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Name: SalesCPick</p></li>
<li><p>Users:</p>
<ul>
<li><p>Kellie Melby</p></li>
<li><p>Sales1@YourFullName##.com</p></li>
<li><p>Sales2@YourFullName##.com</p></li>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2"><p id="p1">4.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Features-&gt; Paging group-&gt; Add New</p></td>
</tr>
<tr>
<td><p id="p2">Anita Perez needs to quickly make important announcements to all employees.</p>
<p>Create a paging group</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Name: Announcements Page</p></li>
<li><p>Extension: 501</p></li>
<li><p>Paging Targets: All employees</p></li>
<li><p>Paging Originators: Anita Perez</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2"><p id="p1">5.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Features -&gt;Voicemail group-&gt; Add New</p></td>
</tr>
<tr>
<td><p id="p2">After hours calls need to route to a voice mailbox that all employees in the Sales and Marketing departments can access</p>
<p>Create a voicemail group</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Name: AfterHours VmailGroup</p></li>
<li><p>Extension: 600</p></li>
<li><p>Passcode: 258011</p></li>
<li><p>Language: English</p></li>
<li><p>Do not make changes to Voicemail Settings</p></li>
</ul>
</td>
</tr>
<tr>
<td rowspan="2"><p id="p1">6.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Features-&gt; Operating Mode-&gt; Add New</p></td>
</tr>
<tr>
<td><p id="p2">Rebekah Barretta needs to route Product Development calls to voicemail during events like unexpected office closures or company-wide meetings.</p>
<p>Create an operating mode</p>
<ul>
<li><p>Level: Organization</p></li>
<li><p>Name: ToMode</p></li>
<li><p>Schedule: None</p></li>
<li><p>Forward destination: Ext 600 (AfterHours VmailGroup)</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2"><p id="p1">7.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Features-&gt; Hunt group-&gt; Add New</p></td>
</tr>
<tr>
<td><p id="p2">During business hours, Marketing  employees need to share the incoming call volume within their groups. Create a hunt group for Marketing</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Name: Marketing HG</p></li>
<li><p>Extensions: 701</p></li>
<li><p>Routing: Longest idle</p></li>
<li><p>Routing Options: Advance when busy</p></li>
<li><p>Assign all Marketing employees and Eric Steele</p></li>
</ul>
<p id="p2">During business hours Product Development employees need to share the incoming call volume within their groups. Create a hunt group for Product Development. Rebekah Barretta needs to activate Operation mode to route calls to voicemail during events like unexpected office closures or company-wide meetings.</p>
<ul>
<li><p>Location: Factory</p></li>
<li><p>Name: ProductDev HG</p></li>
<li><p>Extensions: 701</p></li>
<li><p>Routing: Circular</p></li>
<li><p>Routing Options: Advance when busy</p></li>
<li><p>Assign all ProductDev employees and Rebeka Barretta</p></li>
<li><p>Create HG</p></li>
<li><p>Open HG and open Call Forwarding </p>
<ul>
<li><p>Call Forwarding: Enable</p>
<li><p>Forward calls by mode</p></li>
<li><p>Add ToMode operating mode</p></li>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2"><p id="p1">8.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Features-&gt; Announcements-&gt;
Add New</p></td>
</tr>
<tr>
<td><p id="p2">The company needs to let callers know that certain calls are recorded.</p>
<p>Upload a greeting to be used for specific features</p>
<ul>
<li><p>Upload</p></li>
<li><p>Location: Organization</p></li>
<li><p>Label: All Calls are Recorded</p></li>
<li><p>Download <a href="https://webexcc-sa.github.io/LAB-1251/assets/All-Calls-are-Recorded.wav" download>All-Calls-are-Recorded.wav</a></p></li>
<li><p>Upload: All-Calls-are-Recorded.wav</p></li>
</ul>

<p id="p2">The company wants callers to hear messages periodically while
they are on hold for certain calls.</p>
<p>Record and save a greeting to be used for specific features</p>
<ul>
<li><p>Record</p></li>
<li><p>Location: Organization</p></li>
<li><p>Label: Waiting</p></li>
<li><p>Filename: Answer Soon</p></li>
<li><p>Message: “Your call is important to us. We will be with you shortly”</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2"><p id="p1">9.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Features-&gt; Auto attendant-&gt; Add New</p></td>
</tr>
<tr>
<td><p id="p2">Calls to the Factory main number must be answered by an automated system giving callers the options to reach their desired department with different options for business and after hours</p>
<p>Create an auto attendant for the Factory main number</p>
<ul>
<li><p>Location: Factory</p></li>
<li><p>Name: AA Main</p></li>
<li><p>Phone Number: Factory Main Number (taken from Lab02)</p></li>
<li><p>Extension: 250</p></li>
<li><p>Language: English</p></li>
<li><p>Business Hours Schedule: Open Hours</p></li>
<li><p>Holiday Schedule: None</p></li>
<li><p id="p3">Business Hours Menu</p>
<ul>
<li><p>Disable extension level dialing</p></li>
<li><p>Option 1:Transfer without prompt:Extension 81-701 (Marketing HG)</p></li>
<li><p>Option 2:Transfer without prompt: Extension 82-701 (Product Development Factory)</p></li>
<li><p>Option 3: Repeat Menu</p></li>
<li><p>Option 4: Transfer call to operator – Extension 81-101 (Anita Perez)</p></li>
</ul></li>
<li><p id="p3">After Hours Menu</p>
<ul>
<li><p>Option 1: Transfer call to operator – Extension 81-600 (VmailGroup)</p></ul></li>
</li>
<li><p id="p3">Business Hours Greetings</p>
<ul>
<li><p>Custom Welcome Greeting: Record and rename file to welcome.wav</p></li>
</ul></li>

<li><p id="p3">After Hours Greetings</p>
<ul>
<li><p>Custom Closed Greeting: Record and rename file to closed.wav</p></li>
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