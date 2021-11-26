# Deluge-code-Leads
This Deluge Code execute, when 'Country Field' is 'United States'  changing the country name  as 'U.S.A'


response = zoho.crm.getRecordById("Leads",Lead_ID);
for each  rec in response
{
	info rec.get("id");
	leadid = rec.get("id");
	info leadid;
	mp = Map();
	mp.put("Country","U.S.A");
	updatemylead = zoho.crm.updateRecord("Leads",leadid.tolong(),mp);
	info updatemylead;
}
