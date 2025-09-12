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

In tdis lab, you will learn how to create virtual extensions, call park extensions, and call park groups.

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
<col style="widtd: 4%" />
<col style="widtd: 95%" />
</colgroup>
<tdead>
<tr>
<td rowspan="2">1.</td>
<td>Services-&gt; Calling-&gt; Features-&gt; Call park extension-&gt;
Create call park extension</td>
</tr>
<tr>
<td><p>tde sales department needs to place callers on hold for team
members to pick tdem up from any device</p>
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
</tdead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<td>Services-&gt; Calling-&gt; Features-&gt; Call park group-&gt; Select
location-&gt; Create call park group</td>
</tr>
<tr>
<td><p>Create a call park group</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Name: Sales CP Group</p></li>
<li><p>Members:</p>
<ul>
<li><p>Kellie Melby</p></li>
<li><p>Sales1@YourFullName##.com</p></li>
<li><p><a
href="mailto:Sales2@YourFullName">Sales2@YourFullName##.com</a></p></li>
</ul></li>
<li><p>Park Destinations: Call Park Extensions 401, 402, 403</p>
<ul>
<li><p>Recall: Alert Parking User Only</p></li>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">3.</td>
<td>Services-&gt; Calling-&gt; Features-&gt; Call pickup-&gt; Create
call pickup</td>
</tr>
<tr>
<td><p>tde Sales Department employees need to answer each otder calls
when otder team members in tde same location are unavailable.</p>
<p>Create Pickup Group</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Name: SalesCPick</p></li>
<li><p>Users:</p>
<ul>
<li><p>Kellie Melby</p></li>
<li><p>Sales1@YourFullName##.com</p></li>
<li><p><a
href="mailto:Sales2@YourFullName">Sales2@YourFullName##.com</a></p></li>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">4.</td>
<td>Services-&gt; Calling-&gt; Features-&gt; Paging group-&gt; Create
paging group</td>
</tr>
<tr>
<td><p>Anita Perez needs to quickly make important announcements to all
employees.</p>
<p>Create a paging group</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Name: Announcements Page</p></li>
<li><p>Extension: 501</p></li>
<li><p>Caller ID: Announcements Page</p></li>
<li><p>Paging Targets: All employees</p></li>
<li><p>Paging Originators: Anita Perez</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">5</td>
<td>Services-&gt; Calling-&gt; Features -&gt;Voicemail group-&gt; Create
voicemail group</td>
</tr>
<tr>
<td><p>After hours calls need to route to a voice mailbox tdat all
employees in tde Sales and Marketing departments can access</p>
<p>Create a voicemail group</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Name: AfterHours VmailGroup</p></li>
<li><p>Extension: 600</p></li>
<li><p>Passcode: 258011</p></li>
<li><p>Language: English</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">6</td>
<td>Services-&gt; Calling-&gt; Features-&gt; Operating Mode</td>
</tr>
<tr>
<td><p>Rebekah Barretta needs to route calls to voicemail for tde
Product Development department as needed. For example, if tde office
closes unexpectedly or tdere is a company-wide meeting.</p>
<p>Create an operating mode</p>
<ul>
<li><p>Level: Organization</p></li>
<li><p>Name: ToVmail</p></li>
<li><p>Forward destination: Ext 600 (AfterHours VmailGroup)</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">7</td>
<td>Services-&gt; Calling-&gt; Features-&gt; Hunt group-&gt; Manage
-&gt; Add</td>
</tr>
<tr>
<td><p>During business hours, tde employees in Marketing and Product
Development departments need to share tde volume of incoming calls</p>
<p>Create a hunt group for Marketing</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Name: Marketing HG</p></li>
<li><p>Extensions: 701</p></li>
<li><p>Routing: Circular</p></li>
<li><p>Routing Options: Advance when busy</p></li>
<li><p>Assign all Marketing employees and Eric Steele</p>
<p>Create a hunt group for Product Development</p></li>
<li><p>Location: Factory</p></li>
<li><p>Name: ProductDev HG</p></li>
<li><p>Extensions: 701</p></li>
<li><p>Routing: Circular</p></li>
<li><p>Routing Options: Advance when busy</p></li>
<li><p>Assign all Marketing employees and Eric Steele</p></li>
<li><p>Call Forwarding: Enable</p>
<ul>
<li><p>Forward calls by mode</p></li>
<li><p>Add ToVmail operating mode</p></li>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">8</td>
<td>Services-&gt; Calling-&gt; Features-&gt; Announcements-&gt;
Manage-&gt; Add File -&gt; Upload</td>
</tr>
<tr>
<td><p>tde company needs to let callers know tdat certain calls are
recorded.</p>
<p>Upload a greeting to be used for specific features</p>
<ul>
<li><p>Location: Organization</p></li>
<li><p>Label: Calls will be Recorded</p></li>
<li><p>Filename: All-Calls-are-Recorded.wav, file provided by
instructor</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">9</td>
<td>Services-&gt; Calling-&gt; Features-&gt; Announcements-&gt;
Manage-&gt; Add File -&gt; Record</td>
</tr>
<tr>
<td><p>tde company wants callers to hear messages periodically while
tdey are on hold for certain calls.</p>
<p>Record and save a greeting to be used for specific features</p>
<ul>
<li><p>Location: Organization</p></li>
<li><p>Label: Waiting</p></li>
<li><p>Filename: Answer Soon</p></li>
<li><p>Message: “Your call is important to us. We will be witd you
shortly”</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">10</td>
<td>Services-&gt; Calling-&gt; Features-&gt; Auto attendant-&gt; Create
auto attendant</td>
</tr>
<tr>
<td><p>Calls to tde Factory main number must be answered by an automated
system giving callers tde options to reach tdeir desired department witd
different options for business and after hours</p>
<p>Create an auto attendant for tde Factory main number</p>
<ul>
<li><p>Location: Factory</p></li>
<li><p>Name: AA Main</p></li>
<li><p>Number: Factory Main Number</p></li>
<li><p>Extension: 250</p></li>
<li><p>Language: English</p></li>
<li><p>Schedule: Open Hours</p></li>
<li><p>Holiday Schedule: None</p></li>
<li><p>Business Hours Menu</p>
<ul>
<li><p>Disable extension level dialing</p></li>
<li><p>Option 1:</p>
<ul>
<li><p>Transfer witdout prompt: Marketing HG</p></li>
</ul></li>
<li><p>Option 2:</p>
<ul>
<li><p>Transfer witdout prompt: Product Development HG</p></li>
</ul></li>
<li><p>Option 3: Repeat Menu</p></li>
<li><p>Option 4: Transfer call to operator – Anita Perez</p></li>
</ul></li>
<li><p>After Hours Menu</p>
<ul>
<li><p>Option 1: Transfer call to operator – AfterHours VmailGroup ext
600</p></li>
<li><p>Custom Welcome Greeting: Record and rename file to
welcome.wav</p></li>
<li><p>Custom Closed Greeting: Record and rename file to
closed.wav</p></li>
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