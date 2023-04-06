For this project I created a database to manage the internal audit plan of a large company, including:

Audit teams, managers and individual team members 
Executive management sponsors and key stakeholders 
Audit plan including key milestones, status and final grade for each audit 
Capture the results of post-audit feedback questionnaires
Enable production of management information (MI) and reporting on timescales, team performance, stakeholder interaction and other factors

The database comprises 10 tables in total: two fact tables and eight dimension tables, all normalised to 3NF and with auto incrementing primary keys. 

Scripts created include: 
A stored function used to identify any overdue audits (where the final report has been issued to the sponsor but has not yet been approved)
A stored procedure used to simply recording of responses to post-audit feedback questionnaires 
A trigger to prevent entry of a final report date that precedes the date of the draft report
View to show all in-flight audits with their team, sponsor and milestones
View pulling everything together (apart from feedback) i.e. audit titles, teams, sponsors, stakeholders, milestone dates, status updates etc 
Various queries to use for management reporting including use of time intelligence - demonstrating use of subqueries, concatenation, joins, CTEs, MAX/MIN/AVG/ROUND functions, group by etc 

And finally I created a basic Tableau dashboard to provide management insight on various aspects including a breakdown of grades by executive sponsor (to identify problematic business areas) and by audit manager (to identify whether anyone is particularly harsh or lenient), overview of current status, in-flight audits broken down by team and manager etc. 

Please note that the contents of the database are fictional. 

