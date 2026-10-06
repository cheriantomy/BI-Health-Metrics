# BI-Health-Metrics done during the job at Technology Cue
A Power BI dashboard through automation that monitors the health, adoption, performance and cost
of a Power BI environment, so admins can find unused reports, failing
refreshes and wasted licenses.
<img width="1160" height="690" alt="image" src="https://github.com/user-attachments/assets/d0f763d2-28d3-4301-9529-a247184c200f" />
## Problem
Organizations accumulate reports and workspaces that nobody uses, and refresh
failures go unnoticed. This dashboard makes usage, errors and cost visible in
one place.

## Key questions answered
- Which reports, workspaces and users are active vs inactive?
- Which datasets are slow to refresh, and which jobs fail?
- Which errors happen most often?
- How much does maintaining inactive reports and failed jobs cost per year?
- Where can licenses be saved?

## Key insights
Area	Finding	Recommendation
Workspaces	172 workspaces, 85% are personal (146) and only 26 are corporate. 5 are orphaned and 2 are deleted.	Move shared content to corporate workspaces and assign owners to orphaned ones.
Access rights	Of 284 access assignments, 65% are Admin and only 15% are Viewer.	Apply least-privilege: move most Admins to Member or Viewer.
Refresh reliability	Of 677 refresh records, 88% completed and about 10% failed.	Set up alerts for failed refreshes.
Failure causes	Leading errors are identity and credential issues (user not found in the directory, invalid gateway credentials, credentials not specified).	Review dataset owners and gateway credentials regularly.
Error hotspots	One workspace accounts for 24% of all refresh records, and one report for 61 of them.	Fix a few hotspots to remove much of the noise.
Refresh speed	Average refresh is 5.5 min, median 2.2 min, slowest 27.6 min. 51% of datasets take over 2 minutes.	Optimize queries and models for the slowest datasets.
Schedules	72% of schedules (52 of 72) are disabled.	Review disabled schedules and archive unused reports.
Data sources	67% SQL, 24% SharePoint lists, the rest files and folders.	Prioritize SQL source stability and monitoring.
Usage	38 distinct users, but only 348 report views in the period. About 91% of logged events are automated admin API calls.	Promote adoption and retire reports nobody opens.
Viewing channels	Web 287 views, exports 31, mobile 16, embedded 16.	Web is the main channel, so optimize the experience there.
User security	81% of directory users have "password never expires".	Flag to the security team for policy review.

## Dashboard Preview
- <img width="1181" height="665" alt="image" src="https://github.com/user-attachments/assets/4a8159dd-5f48-4cec-8edb-5026e491c80c" />
- <img width="1171" height="662" alt="image" src="https://github.com/user-attachments/assets/f5a4ab94-2b97-4996-a131-8b264353e222" />
- <img width="1176" height="662" alt="image" src="https://github.com/user-attachments/assets/191602f6-5a09-45cf-9ed0-b648284c7b45" />
- <img width="1097" height="611" alt="image" src="https://github.com/user-attachments/assets/b18db73b-a397-4f84-a481-2a910a71e4f7" />
- <img width="1175" height="662" alt="image" src="https://github.com/user-attachments/assets/1648ed28-df28-425c-92c9-a568d46684bd" />
- <img width="1172" height="662" alt="image" src="https://github.com/user-attachments/assets/b849f4d2-0f8e-447b-9128-4950fc280b70" />
- <img width="1177" height="657" alt="image" src="https://github.com/user-attachments/assets/11261039-cf67-4cd7-86a1-38d51dc26401" />
- <img width="1171" height="662" alt="image" src="https://github.com/user-attachments/assets/7825bfd5-3cd1-4bcb-8222-a99c4b83816c" />
- <img width="1172" height="665" alt="image" src="https://github.com/user-attachments/assets/29ad6a68-aae2-4226-92bb-0b28592a623d" />
- <img width="1182" height="662" alt="image" src="https://github.com/user-attachments/assets/82ac766a-a25a-428e-951b-fcd5056cd49c" />

## ## Tools used
Power BI Desktop, DAX, Power Query, Power BI REST / Admin APIs, SQL











