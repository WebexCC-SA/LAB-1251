

LAB–1251

Leveling up communication: A follow-along Webex Calling lab​

This hands-on lab provides experience in Webex Calling. Complete
practical exercises such as configuring local gateways, using features,
and managing call routing through Webex Control Hub. Learn to handle
calls efficiently, explore mid-call functions, and understand call flow
management in a simulated environment. The lab enhances skills in
managing communication systems and optimizes telephony infrastructure
for improved organizational communication.

# Table of Contents

[Lab Guide: Getting started
[4](#lab-guide-getting-started)](#lab-guide-getting-started)

[Customer Scenario [4](#customer-scenario)](#customer-scenario)

[Lab 1 – Organization Settings
[5](#lab-1-organization-settings)](#lab-1-organization-settings)

[Lab 2 – Location Settings
[6](#lab-2-location-settings)](#lab-2-location-settings)

[Lab 3 – Users [9](#lab-3-users)](#lab-3-users)

[Lab 4 – Devices [11](#lab-4-devices)](#lab-4-devices)

[Lab 5 – Workspaces [12](#lab-5-workspaces)](#lab-5-workspaces)

[Lab 6 – Virtual and shared lines
[14](#lab-6-virtual-and-shared-lines)](#lab-6-virtual-and-shared-lines)

[Lab 7 – Configuring Calling features
[15](#lab-7-configuring-calling-features)](#lab-7-configuring-calling-features)

[Lab 8 – Creating Call Queues
[19](#lab-8-creating-call-queues)](#lab-8-creating-call-queues)

[Lab 9 – Admin-controlled user features
[21](#lab-9-admin-controlled-user-features)](#lab-9-admin-controlled-user-features)

[Lab 10 – Configurations in User Hub
[22](#lab-10-configurations-in-user-hub)](#lab-10-configurations-in-user-hub)

# Lab Guide: Getting started

This guide is structured into multiple labs, each focusing on a specific
aspect of Webex Calling configuration. To successfully complete the
exercises:

- Follow Steps Sequentially

  - Numbered steps must be followed precisely

  - If a setting in Control Hub is not listed in the task instructions,
    leave default settings or skip

- Access URLs and Login

  - Use specified URLs (e.g., \`admin.webex.com\`) for portals

  - Instructor-provided login credentials

  - Ensure correct login for each task

  - Green text = Online navigation for the portal in use

- End of each lab section marked by "STOP – END OF LAB”

  - Wait for further instruction before moving forward

## Customer Scenario

This lab guide provides step-by-step instructions for configuring Webex
Calling to meet the business needs of our fictional customer, Paw Pet
Supply Solutions, who are new to the platform.

#### Company Profile

- Paw Pet Supply Solutions is an emerging leader in the pet supply
  industry

- Provides high-quality, innovative products for pet care

- Committed to animal well-being and customer satisfaction

- Aims to be a trusted partner for pet parents

#### Setup and Requirements

- Locations: HQ in California, Factory in Texas

- Communication Platform: Webex Calling with Cisco Calling Plan as PSTN
  solution

- Departments: Marketing, Sales, Product Development

- Numbers: Main number for Sales, Auto Attendant for Marketing and
  Product Development

- Business Hours: 9 am – 5 pm, voicemail after hours

- Sales Department Specifics: Call pickup, call hold for department
  members, company-wide announcements

- Product Development Specifics: User-controlled voicemail routing

- Shared Resources: Shared Cubicles at HQ, Conference rooms with Room
  Board devices and phones, all employees use MPP phones.

- Pre-configured Environment: Foundational elements already created for
  streamlined experience:

- One location: “dCloud”, to be renamed

- Eight users: one administrator, seven standard users.

- All users require Webex Calling licenses

# Lab 1 – Organization Settings

In this lab, you will learn how to navigate and configure organization
settings for Webex Calling.

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials: Charles Holland – Webex Administrator

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th>Services-&gt; Calling-&gt; Service settings-&gt; Internal
dialing-&gt; Edit</th>
</tr>
<tr>
<th><p>All location extensions are mirror images of each other</p>
<p>Enable an internal dialing plan at the organization level</p>
<ul>
<li><p>Routing prefix length: 2</p></li>
<li><p>Steering digit: 8</p></li>
<li><p>Extension length: 3</p></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<td>Services-&gt; Calling-&gt; Service settings-&gt; Voicemail</td>
</tr>
<tr>
<td><p>A default passcode is required for new voicemail users</p>
<p>Set a default voicemail passcode for all users in the
organization</p>
<ul>
<li><p>Default Passcode: 258011</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">3.</td>
<td>Services-&gt; Calling-&gt; Service settings-&gt; Call Recording</td>
</tr>
<tr>
<td><p>Webex is the preferred calling vendor</p>
<p>Set Webex as the call recording provider</p></td>
</tr>
</tbody>
</table>

STOP - END OF LAB

<img src="media/image7.svg" style="width:1.27778in;height:1.27778in"
alt="Stop with solid fill" />

# Lab 2 – Location Settings

In this lab, you will learn how to add locations.

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials: Charles Holland – Webex Administrator

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th>Management-&gt; Locations-&gt; dCloud-&gt; Location info</th>
</tr>
<tr>
<th><p>San Jose is the headquarters and main location</p>
<p>Rename dCloud location</p>
<ul>
<li><p>Location name: HQ</p></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<td>Management-&gt; Locations-&gt; Manage location-&gt; Create
manually</td>
</tr>
<tr>
<td><p>Paw Pet Solutions has a factory in Houston, TX.</p>
<p>Add a location</p>
<ul>
<li><p>Location name: Factory</p></li>
<li><p>Address: 4501 North Main Street, Houston, TX 77009, USA</p></li>
<li><p>Time zone: Chicago</p></li>
<li><p>Country – USA</p></li>
<li><p>Language – English</p></li>
<li><p>Click “Set up calling” after creating your location and then
close the PSTN connection window.</p>
<ul>
<li><p>You will set up the PSTN connection in another step</p></li>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">3.</td>
<td>Management-&gt; Locations-&gt; Select location-&gt; Calling-&gt;
PSTN connection</td>
</tr>
<tr>
<td><p>HQ and Factory will use the Cisco Calling Plan</p>
<p>Assign a PSTN Connection to each location</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Connection Type: Cisco Calling Plans</p></li>
<li><p>Contract Information: Your name, Student login email
address</p></li>
<li><p>Services Address: HQ location address (already entered)</p></li>
<li><p>Authorized Contact: Your name</p></li>
<li><p>Job title: Admin</p>
<p>Repeat steps for Factory location</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">4.</td>
<td>Services-&gt; Calling-&gt; Numbers-&gt; Manage-&gt; Add</td>
</tr>
<tr>
<td><p>Each location needs 10 numbers</p>
<p>Add Numbers</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Number Type: PSTN</p></li>
<li><p>Select an Area Code from the list</p></li>
<li><p>Select 10 numbers</p></li>
<li><p>Click view orders</p></li>
<li><p>Click on the pending order to automatically change the status to
provisioned</p>
<p>Repeat steps for Factory location</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">5.</td>
<td>Management-&gt; Locations-&gt; Select location -&gt; Calling-&gt;
Calling Connection-&gt; Main number</td>
</tr>
<tr>
<td><p>To make and receive calls each location needs a main number. Each
location must present their own main number as their caller id.</p>
<p>Assign a main number to each location</p>
<ul>
<li><p>Select any of the available numbers</p></li>
<li><p>You will need to know these numbers in a subsequent lab; make a
note of which ones you use</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">6.</td>
<td>Management-&gt; Locations-&gt; Select location -&gt; Calling-&gt;
Dialing-&gt; Internal dialing</td>
</tr>
<tr>
<td><p>All location extensions are mirror images of each other.</p>
<p>Add a routing prefix for each location</p>
<ul>
<li><p>HQ: 81</p></li>
<li><p>Factory: 82</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">7.</td>
<td>Management-&gt; Locations-&gt; Select location -&gt; Calling-&gt;
Calling feature settings-&gt; Voice portal</td>
</tr>
<tr>
<td><p>All locations need voicemail.</p>
<p>Configure the voice portal for each location</p>
<ul>
<li><p>Extension: 200</p></li>
<li><p>Voice Portal Admin Passcode: 137041</p></li>
<li><p>Language: English</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">8.</td>
<td>Management-&gt; Locations-&gt; Select location -&gt; Calling-&gt;
Calling feature settings-&gt; Schedules</td>
</tr>
<tr>
<td><p>Calls coming into the main numbers need to route to specific
options based on the time of day.</p>
<p>Create a schedule for both locations</p>
<ul>
<li><p>Name: Open Hours</p></li>
<li><p>Schedule Type: Business Hours</p></li>
<li><p>Monday – Friday 9:00 am – 5 pm</p></li>
</ul></td>
</tr>
</tbody>
</table>

STOP - END OF LAB

<img src="media/image7.svg" style="width:1.27778in;height:1.27778in"
alt="Stop with solid fill" />

# Lab 3 – Users

In this lab, you will learn how to create users, assign licenses, and
assign extensions to users manually and in bulk.

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials: Charles Holland – Webex Administrator

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th>Management-&gt; Users-&gt; select user</th>
</tr>
<tr>
<th><p>Anita Perez needs a phone number and to use calling features.</p>
<p>Assign Anita a Calling license and assign a phone number</p>
<ul>
<li><p>License: Webex Calling Professional</p></li>
<li><p>Location: HQ</p></li>
<li><p>Number: Unused number (not main number of the Location)</p></li>
<li><p>Extension: 101</p></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<td>Management-&gt; Users-&gt; Manage users-&gt; Add users-&gt; Manually
add users OR CSV add or edit</td>
</tr>
<tr>
<td><p>There are 16 employees that require extensions for calling.</p>
<ul>
<li><p>Use instructor provided Add Users and Devices Template file or
tables below</p>
<ul>
<li><p>YourFullName = Your first and last name</p></li>
<li><p>## = Instructor provided student number</p></li>
</ul></li>
<li><p>Create users for each location manually and/or in bulk</p></li>
<li><p>Assign a Webex Calling professional license and an extension
number</p></li>
</ul></td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 53%" />
<col style="width: 20%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr>
<th>HQ User Emails</th>
<th>Extensions</th>
<th>License</th>
</tr>
</thead>
<tbody>
<tr>
<td>Charles Holland</td>
<td>102</td>
<td>Professional</td>
</tr>
<tr>
<td>Eric Steele</td>
<td>103</td>
<td>Professional</td>
</tr>
<tr>
<td>Kellie Melby</td>
<td>104</td>
<td>Professional</td>
</tr>
<tr>
<td>Sales1@YourFullName##.com</td>
<td>105</td>
<td>Professional</td>
</tr>
<tr>
<td>Sales2@YourFullName##.com</td>
<td>106</td>
<td>Professional</td>
</tr>
<tr>
<td>Marketing1@YourFullName##.com</td>
<td>107</td>
<td>Professional</td>
</tr>
<tr>
<td>Marketing2@YourFullName##.com</td>
<td>108</td>
<td>Professional</td>
</tr>
</tbody>
</table>

<table>
<colgroup>
<col style="width: 53%" />
<col style="width: 20%" />
<col style="width: 25%" />
</colgroup>
<thead>
<tr>
<th>Factory User Emails</th>
<th>Extensions</th>
<th>License</th>
</tr>
</thead>
<tbody>
<tr>
<td>Ricardo Filice</td>
<td>101</td>
<td>Professional</td>
</tr>
<tr>
<td>Stefan Mauk</td>
<td>102</td>
<td>Professional</td>
</tr>
<tr>
<td>Taylor Bard</td>
<td>103</td>
<td>Professional</td>
</tr>
<tr>
<td>Rebekah Barretta</td>
<td>104</td>
<td>Professional</td>
</tr>
<tr>
<td>ProductDev1@YourFullName##.com</td>
<td>105</td>
<td>Professional</td>
</tr>
<tr>
<td>ProductDev 2@YourFullName##.com</td>
<td>106</td>
<td>Professional</td>
</tr>
<tr>
<td>ProductDev 3@YourFullName##.com</td>
<td>107</td>
<td>Professional</td>
</tr>
<tr>
<td>ProductDev 4@YourFullName##.com</td>
<td>108</td>
<td>Professional</td>
</tr>
</tbody>
</table>

STOP - END OF LAB

<img src="media/image7.svg" style="width:1.27778in;height:1.27778in"
alt="Stop with solid fill" />

# Lab 4 – Devices

In this lab, learn how to assign devices to users.

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials: Charles Holland – Webex Administrator

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th>Devices-&gt; Add device-&gt; Personal Usage OR Multiple Cisco IP
Phones</th>
</tr>
<tr>
<th><p>All users have a Cisco <mark>8800</mark> series phone</p>
<ul>
<li><p>Use instructor provided Add Users and Devices Template file or
tables below</p>
<ul>
<li><p>Assign devices to users manually or in bulk</p></li>
</ul></li>
<li><p>Activation method: Activation Code</p></li>
<li><p>Do not include extension numbers in the CSV file</p></li>
<li><p>Type: USER</p></li>
<li><p>Device Type: IP</p></li>
<li><p>Model: Cisco <mark>8865</mark></p></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

STOP - END OF LAB

<img src="media/image7.svg" style="width:1.27778in;height:1.27778in"
alt="Stop with solid fill" />

# Lab 5 – Workspaces

In this lab, you will learn how to create workspaces, assign devices to
workspaces, and enable hoteling and hotdesking on workspace devices.

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials: Charles Holland – Webex Administrator

<table>
<colgroup>
<col style="width: 6%" />
<col style="width: 93%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th>Management-&gt; Workspaces-&gt; Add Workspace</th>
</tr>
<tr>
<th><p>Paw Pet Supply Solutions has 4 shared use areas in which they
need to hold meetings and make and receive calls</p>
<ul>
<li><p>Add the workspaces with the corresponding devices and
services</p></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td colspan="2"><table>
<colgroup>
<col style="width: 18%" />
<col style="width: 10%" />
<col style="width: 13%" />
<col style="width: 33%" />
<col style="width: 11%" />
<col style="width: 12%" />
</colgroup>
<thead>
<tr>
<th>Workspace name</th>
<th>Type</th>
<th>Device</th>
<th>Services</th>
<th>Location</th>
<th>Extension</th>
</tr>
</thead>
<tbody>
<tr>
<td>SharedCubicle1</td>
<td>Desk</td>
<td>Cisco Desk Phone - 9841</td>
<td><p>Cisco Webex Calling</p>
<p>Common area workspace</p></td>
<td>HQ</td>
<td>201</td>
</tr>
<tr>
<td>SharedCubicle2</td>
<td>Desk</td>
<td><mark>Cisco 8865</mark></td>
<td><p>Cisco Webex Calling</p>
<p>Common area workspace</p></td>
<td>HQ</td>
<td>201</td>
</tr>
<tr>
<td rowspan="2">Conference Room1</td>
<td rowspan="2">Meeting Room</td>
<td>Cisco Board Pro</td>
<td rowspan="2">Cisco Webex Calling Professional workspace</td>
<td rowspan="2">HQ</td>
<td rowspan="2">300</td>
</tr>
<tr>
<td><mark>Cisco</mark> <mark>8865</mark></td>
</tr>
<tr>
<td rowspan="2">Conference Room1</td>
<td rowspan="2">Meeting Room</td>
<td>Cisco Board Pro</td>
<td rowspan="2">Cisco Webex Calling Professional workspace</td>
<td rowspan="2">Factory</td>
<td rowspan="2">300</td>
</tr>
<tr>
<td><mark>Cisco</mark> <mark>8865</mark></td>
</tr>
</tbody>
</table></td>
</tr>
<tr>
<td rowspan="2">2.</td>
<td>Management-&gt; Workspaces-&gt; Select Workspace-&gt;
Scheduling</td>
</tr>
<tr>
<td><p>To conduct calls in private, users may sometimes need to access
all of their configured lines from a location other than their usual
desk.</p>
<p>Enable Hot Desking</p>
<ul>
<li><p>Workspace: SharedCubicle1</p></li>
<li><p>Hot Desking: Enable</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">3</td>
<td>Management-&gt; Devices-&gt; Select device-&gt; Hoteling</td>
</tr>
<tr>
<td><p>To conduct calls in private, users may sometimes need to make and
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

STOP - END OF LAB

<img src="media/image7.svg" style="width:1.27778in;height:1.27778in"
alt="Stop with solid fill" />

# Lab 6 – Virtual and shared lines

Learn how to create virtual lines and assign them as shared line
appearances.

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials: Charles Holland – Webex Administrator

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th>Services-&gt; Calling-&gt; Virtual Lines</th>
</tr>
<tr>
<th><p>Eric Steele and Kellie Melby require a Houston phone number for
calling customers in the Houston area</p>
<p>Create two virtual lines</p>
<ul>
<li><p>Names: Extra Line1 and Extra Line2</p></li>
<li><p>Location: Factory</p></li>
<li><p>Assign a spare phone number and extension 110 and 111</p></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<td>Management-&gt; Devices-&gt; Select device-&gt; Device Management
-&gt; Configure Lines</td>
</tr>
<tr>
<td><p>Eric Steele and Kellie will need to access those lines on their
8800 series Cisco multi-platform phones</p>
<p>Assign virtual lines from the step above to the appropriate
devices</p></td>
</tr>
</tbody>
</table>

STOP

<img src="media/image9.svg" style="width:1in;height:1in"
alt="Warning outline" />

STOP - END OF LAB

# Lab 7 – Configuring Calling features

In this lab, you will learn how to create virtual extensions, call park
extensions, and call park groups.

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials: Charles Holland – Webex Administrator

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th>Services-&gt; Calling-&gt; Features-&gt; Call park extension-&gt;
Create call park extension</th>
</tr>
<tr>
<th><p>The sales department needs to place callers on hold for team
members to pick them up from any device</p>
<p>Create call park extensions</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Names &amp; Extensions:</p>
<ul>
<li><p>Extension 1 – 401</p></li>
<li><p>Extension 2 – 402</p></li>
<li><p>Extension 3 – 403</p></li>
</ul></li>
</ul></th>
</tr>
</thead>
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
<td><p>The Sales Department employees need to answer each other calls
when other team members in the same location are unavailable.</p>
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
<td><p>After hours calls need to route to a voice mailbox that all
employees in the Sales and Marketing departments can access</p>
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
<td><p>Rebekah Barretta needs to route calls to voicemail for the
Product Development department as needed. For example, if the office
closes unexpectedly or there is a company-wide meeting.</p>
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
<td><p>During business hours, the employees in Marketing and Product
Development departments need to share the volume of incoming calls</p>
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
<td><p>The company needs to let callers know that certain calls are
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
<td><p>The company wants callers to hear messages periodically while
they are on hold for certain calls.</p>
<p>Record and save a greeting to be used for specific features</p>
<ul>
<li><p>Location: Organization</p></li>
<li><p>Label: Waiting</p></li>
<li><p>Filename: Answer Soon</p></li>
<li><p>Message: “Your call is important to us. We will be with you
shortly”</p></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">10</td>
<td>Services-&gt; Calling-&gt; Features-&gt; Auto attendant-&gt; Create
auto attendant</td>
</tr>
<tr>
<td><p>Calls to the Factory main number must be answered by an automated
system giving callers the options to reach their desired department with
different options for business and after hours</p>
<p>Create an auto attendant for the Factory main number</p>
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
<li><p>Transfer without prompt: Marketing HG</p></li>
</ul></li>
<li><p>Option 2:</p>
<ul>
<li><p>Transfer without prompt: Product Development HG</p></li>
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

STOP - END OF LAB

<img src="media/image7.svg" style="width:1.27778in;height:1.27778in"
alt="Stop with solid fill" />

# Lab 8 – Creating Call Queues

In this lab, you will learn how to create call queues.

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials: Charles Holland – Webex Administrator

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th>Services-&gt; Calling-&gt; Features-&gt; Call Queue-&gt; Manage
-&gt; Add</th>
</tr>
<tr>
<th><p>During business hours, callers to the San Jose Support and Sales
departments should be placed on hold until an agent is available.</p>
<p>Create a Call Queue</p>
<ul>
<li><p>Location: HQ</p></li>
<li><p>Name: Sales Queue</p></li>
<li><p>Extension: 900</p></li>
<li><p>Number of calls in queue: 15</p></li>
<li><p>Caller ID: Location number</p></li>
<li><p>Routing: Priority Based - Longest Idle</p></li>
<li><p>Overflow: Transfer to Anita Perez after 60 seconds</p></li>
<li><p>Welcome Message: Mandatory</p>
<ul>
<li><p>Custom Welcome Message: Call Recorded, instructor
provided</p></li>
</ul></li>
<li><p>Comfort Message: 20 seconds between messages</p>
<ul>
<li><p>Custom Comfort Message: Answer Soon, instructor provided</p></li>
</ul></li>
<li><p>Hold Music: Play default music</p></li>
<li><p>Agents:</p>
<ul>
<li><p>Sales1@YourFullName##.com</p></li>
<li><p><a
href="mailto:Sales2@YourFullName">Sales2@YourFullName##.com</a></p></li>
<li><p>Eric Steele</p></li>
<li><p>Kellie Melby</p></li>
</ul></li>
<li><p>Enable Night Service:</p>
<ul>
<li><p>Default Greeting</p></li>
<li><p>Transfer to Phone number 600</p></li>
<li><p>Open Hours schedule</p></li>
</ul></li>
<li><p>Stranded calls: Follow Night Service</p></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<td>Services-&gt; Calling-&gt; Features-&gt; Call queue-&gt;
Supervisors-&gt; Add Supervisor</td>
</tr>
<tr>
<td><p>The supervisor needs to silently monitor agents in their
respective queues</p>
<ul>
<li><p>Supervisor: Charles Holland</p></li>
<li><p>Agents:</p>
<ul>
<li><p>Sales1@YourFullName##.com</p></li>
<li><p><a
href="mailto:Sales2@YourFullName">Sales2@YourFullName##.com</a></p></li>
<li><p>Eric Steele</p></li>
<li><p>Kellie Melby</p></li>
</ul></li>
</ul></td>
</tr>
</tbody>
</table>

STOP - END OF LAB

<img src="media/image7.svg" style="width:1.27778in;height:1.27778in"
alt="Stop with solid fill" />

# Lab 9 – Admin-controlled user features

In this lab, you will learn to configure admin-controlled user features.

URL: [admin.webex.com](http://admin.webex.com/) Login: Instructor
provided credentials: Charles Holland – Webex Administrator

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th>Management-&gt; Users-&gt; Rebekah Barretta-&gt; Calling-&gt;
Calling handling -&gt; Mode management</th>
</tr>
<tr>
<th><p>Rebekah Barretta needs to change the Product Development HQ to
ToVmail operating mode as needed</p>
<p>Enable mode management for Rebekah Barretta</p>
<ul>
<li><p>Add Product Development HQ</p>
<p><em>Make note of Rebekah’s email address for the next
lab!</em></p></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<td>Management-&gt; Users-&gt; Anita Perez-&gt; Calling-&gt;
Between-user permissions-&gt; Monitoring</td>
</tr>
<tr>
<td><p>Anita Perez requires the ability to monitor the lines all sales
employees</p>
<p>Add monitored lines to Anita Perez’s profile</p>
<ul>
<li><p>Users:</p>
<ul>
<li><p>Sales1@YourFullName##.com</p></li>
<li><p><a
href="mailto:Sales2@YourFullName">Sales2@YourFullName##.com</a></p></li>
<li><p>Eric Steele</p></li>
<li><p>Kellie Melby</p></li>
</ul></li>
</ul></td>
</tr>
<tr>
<td rowspan="2">3.</td>
<td>Management-&gt; Users-&gt; Anita Perez-&gt; Calling-&gt;
Between-user permissions -&gt; Hotdesking</td>
</tr>
<tr>
<td><p>Anita Perez needs to use a line with a Houston phone number
(virtual line created in Lab 6) when using the Hotdesking feature</p>
<p>Add virtual line to Anita Perez’s profile</p>
<ul>
<li><p>Add: Extra Line1</p></li>
</ul></td>
</tr>
</tbody>
</table>

STOP - END OF LAB

<img src="media/image7.svg" style="width:1.27778in;height:1.27778in"
alt="Stop with solid fill" />

# Lab 10 – Configurations in User Hub

In this lab, you will learn how users can configure calling settings in
User Hub.

URL: [user.webex.com](https://user.webex.com/)

Login: Rebekah Barretta’s email, password same as your admin login
(Charles Holland)

<table>
<colgroup>
<col style="width: 4%" />
<col style="width: 95%" />
</colgroup>
<thead>
<tr>
<th rowspan="2">1.</th>
<th>user.webex.com-&gt; Settings -&gt; Calling -&gt; Features -&gt; Mode
Management</th>
</tr>
<tr>
<th><p>Rebekah Barretta needs to route calls to voicemail for the
Product Development department as needed. For example, if the office
closes unexpectedly or there is a company-wide meeting.</p>
<p>Manage call-forwarding settings in User Hub</p>
<ul>
<li><p>Select Product Development HG</p>
<ul>
<li><p>Switch Mode</p>
<ul>
<li><p>ToVmail</p></li>
</ul></li>
<li><p>Switch back</p></li>
</ul></li>
</ul></th>
</tr>
</thead>
<tbody>
<tr>
<td rowspan="2">2.</td>
<td>user.webex.com -&gt; Settings -&gt; Calling -&gt; Hoteling</td>
</tr>
<tr>
<td><p>Rebekah Barretta sometimes needs to use a phone at the San Jose
location as her own when she visits</p>
<p>Enable hoteling for Rebekah Barretta</p>
<ul>
<li><p>Hoteling: SharedCubicle2</p></li>
</ul></td>
</tr>
</tbody>
</table>

STOP - END OF LAB

<img src="media/image7.svg" style="width:1.27778in;height:1.27778in"
alt="Stop with solid fill" />

Congratulations!

You have completed:

LAB-1251

Leveling up communication:

A follow-along Webex Calling lab
