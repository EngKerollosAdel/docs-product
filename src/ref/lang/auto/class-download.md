---
summary: Explore file sending features and properties of the Download Tool in OutSystems 11 (O11).
locale: en-us
guid: 6db67bd3-800f-40ea-8b86-c545c9a3c2c7
app_type: traditional web apps, mobile apps, reactive web apps
platform-version: o11
figma:
tags: file management, file download, web development, outsystems platform, ajax
audience:
  - mobile developers
  - frontend developers
  - full stack developers
outsystems-tools:
  - service studio
coverage-type:
  - remember
---

# Download

Use the Download Tool to send a file to a user. This is an element that ends the action flow, so it is not possible to define new actions after it. If the Ajax Submit method is used to trigger the download, the download will not work. This includes Links and Buttons with the method type Ajax Submit, or On Click events of other element types, such as Containers.

## Properties

<table markdown="1">
<thead>
<tr>
<th>Name</th>
<th>Description</th>
<th>Mandatory</th>
<th>Default value</th>
<th>Observations</th>
</tr>
</thead>
<tbody>
<tr>
<td title="File Content">File Content</td>
<td>Holds the file selected by the user.</td>
<td>Yes</td>
<td></td>
<td></td>
</tr>
<tr>
<td title="File Name">File Name</td>
<td>Text literal or expression with the name of the file, including the extension.</td>
<td>Yes</td>
<td></td>
<td></td>
</tr>
<tr>
<td title="Mime-Type">Mime-Type</td>
<td>Text literal or expression specifying the media type of the file.</td>
<td>Yes</td>
<td>"application/octet-stream"</td>
<td>Example values:<br/>
– "application/x-msexcel";<br/>
– "application/msword";<br/>
– "application/pdf";<br/>
– "image/gif";<br/>
– "text/html";<br/>
– "video/avi";<br/>
– "audio/wav".</td>
</tr>
<tr>
<td title="Save to Disk">Save to Disk</td>
<td>Set to Yes to allow the user to open or save the file.</td>
<td>Yes</td>
<td>Yes</td>
<td></td>
</tr>
</tbody>
</table>

