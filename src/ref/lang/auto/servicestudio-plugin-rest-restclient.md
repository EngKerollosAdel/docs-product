---
summary: OutSystems 11 (O11) provides a REST API with customizable properties for integration and runtime adjustments.
helpids: 17200
locale: en-us
guid: 750da14a-1a1d-48fd-bea4-735d992e3d48
app_type: traditional web apps, mobile apps, reactive web apps
platform-version: o11
figma:
tags: rest api, integration, api properties, runtime configuration, environment management
audience:
  - mobile developers
  - frontend developers
  - full stack developers
outsystems-tools:
  - service studio
coverage-type:
  - remember
---

# REST API

API to consume information from another system through REST.  

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
<td title="Name">Name</td>
<td>Identifies an element in the scope where it is defined, like a screen, action, or module.</td>
<td>Yes</td>
<td></td>
<td></td>
</tr>
<tr>
<td title="Description">Description</td>
<td>Text that documents the element.</td>
<td></td>
<td></td>
<td>Useful for documentation purpose.<br/>The maximum size of this property is 2000 characters.</td>
</tr>
<tr>
<td title="Image">Icon</td>
<td>Picture to be displayed to help identify this element.</td>
<td>Yes</td>
<td></td>
<td></td>
</tr>
<tr>
<td title="Base URL">Base URL</td>
<td>The base URL of all methods of the REST API.
This value can be customized at runtime in the environment management console.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr >
<th colspan="5">Basic Authentication</th>
</tr>
<tr>
<td title="Username">Username</td>
<td>Username sent in the Authorization header of all methods for Basic Authentication. Can be customized at runtime in the environment console.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td title="Password">Password</td>
<td>Password sent in the Authorization header of all methods for Basic Authentication. Can be customized at runtime in the environment console.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr >
<th colspan="5">Advanced</th>
</tr>
<tr>
<td title="DateFormat">Date Format</td>
<td>Date format used by the Web Service.</td>
<td>Yes</td>
<td>2014-01-01T00:00:00Z (ISO)</td>
<td></td>
</tr>
<tr>
<td title="OnBeforeRequestCallback">On Before Request</td>
<td>The action to customize the request before sending it.</td>
<td></td>
<td></td>
<td>This callback action is useful to debug and customize requests.</td>
</tr>
<tr>
<td title="OnAfterResponseCallback">On After Response</td>
<td>The action to customize the response before it is processed.</td>
<td></td>
<td></td>
<td>This callback action is useful to debug and customize responses.</td>
</tr>
</tbody>
</table>

