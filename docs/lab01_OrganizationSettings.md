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



# Lab 1 - Organization Settings

In this lab, you will learn how to navigate and configure organization settings for Webex Calling.

- Paw Pet Supply Solutions desire their telephone system configured in a certain way: 

    * Control Hub Configuration easy, with a longer timeout
    * Extensions with the XX-XXX format, with mirrored extensions
    * Default passcode for voicemail
    * Call Recording with Webex


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
<td rowspan="2" ><p id="p1">1.</p></td>
<td><p id="p1">Management-&gt; Organization Settings-&gt; Control Hub Idle Timeout</p></td>
</tr>
<tr>
<td><p id="p2">You do not want to be logged out of Control Hub every 20 minutes</p>
<ul>
<li><p>Change the timeout to 12 hours</p></li>
</ul>
<p class="right-aligned"><a href="https://help.webex.com/en-us/article/nl4m0jo/Configure-Idle-Session-Timeout-for-Control-Hub-Users">Webex Help Article</a></p>
</td>
</tr>

<tr>
<td rowspan="2" ><p id="p1">2.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Settings-&gt; Service-&gt; Internal dialing-&gt; Edit </p></td>
</tr>
<tr>
<td><p id="p2">All location extensions are mirror images of each other</p>
<p>Enable an internal dialing plan at the organization level</p>
<ul>
<li><p>Routing prefix length: 2</p></li>
<li><p>Steering digit: 8</p></li>
<li><p>Extension length: 3</p></li>
</ul></td>
</tr>




<tr>
<td rowspan="2"><p id="p1">3.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Settings-&gt; Service-&gt; Voicemail</p></td>
</tr>
<tr>
<td><p id="p2">A default passcode is required for new voicemail users</p>
<p>Set a default voicemail passcode for all users in the
organization</p>
<ul>
<li><p>Default Passcode: 258011</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2"><p id="p1">4.</p></td>
<td><p id="p1">Services-&gt; Calling-&gt; Settings-&gt; Service-&gt; Call Recording</p></td>
</tr>
<tr>
<td><p id="p2">Webex is the preferred calling vendor</p>
<p>Set Webex as the call recording provider</p></td>
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