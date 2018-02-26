---
layout: default
permalink: /scored-legislation
title: Scored Legislation
---

# Open Data Legislation
## Detailed Existing Open Data Legislation
Go back to the <a target="_blank" href="/legislation">Summary of Existing Open Data Legislation</a>, <a target="_blank" href="/detailed-legislation">Detailed Existing Open Data Legislation</a>, and <a target="_blank" href="/scoring">ODI Scoring methodology.</a>
<table cellpadding="10" border="1">
	<tr>
		<th>Session</th>
		<th>Bill Number</th>
		<th>Title</th>
		<th>Organization</th>
		<th>Total Score</th>
		<th>Score Public Default</th>
		<th>Score Tech Standards</th>
		<th>Score Accounting Standards</th>
		<th>Score Metadata Standards</th>
		<th>Score Annual Report</th>
		<th>Score Bi-Annual Report</th>
		<th>Score Incentives</th>
		<th>Score Passed House</th>
		<th>Score Passed Senate</th>
		<th>Score Signed Law</th>
	</tr>
{% for name in site.data.legislation %}
{% assign score = name.public-default | plus: name.tech-standards | plus: name.accounting-standards | plus: name.metadata-standards | plus: name.annual-report | plus: name.bi-annual-meetings | plus: name.incentives | plus: name.passed-house | plus: name.passed-senate | plus: name.signed-law | round: 1 %}
  <tr>
  	<td width="06%" align="center">{{ name.session }}</td>
  	<td width="06%" align="center">{{ name.bill-number }}</td>
  	<td width="17%" align="center">{{ name.title }}</td>
  	<td width="06%" align="center">{{ name.organization }}</td>
  	<td width="05%" align="center">{{ score }}</td>
  	<td width="05%" align="center">{{ name.public-default }}</td>
  	<td width="05%" align="center">{{ name.tech-standards }}</td>
  	<td width="05%" align="center">{{ name.accounting-standards }}</td>
  	<td width="05%" align="center">{{ name.metadata-standards }}</td>
  	<td width="05%" align="center">{{ name.annual-report }}</td>
  	<td width="05%" align="center">{{ name.bi-annual-meetings }}</td>
  	<td width="05%" align="center">{{ name.incentives }}</td>
  	<td width="05%" align="center">{{ name.passed-house }}</td>
  	<td width="05%" align="center">{{ name.passed-senate }}</td>
  	<td width="05%" align="center">{{ name.signed-law }}</td>
  </tr>
{% endfor %}
</table>

**<a target="_blank" href="https://github.com/opendatainitiative/opendatalegislation/tree/0.4">revision 0.4</a>**
