# Salesforce
Case cs = new Case ();

cs.Status = 'In Progress';
cs.Type = 'Emmergency';
cs.Priority = 'High';
cs.Reason = 'Performance Down';
cs.Origin = 'Phone';
cs.Subject = 'My Webcame problem';
cs.Description = 'Dear custumer, My webcame is not working';

cs.Account = '00015000smbboAAb';
Insert cs;
If (cs.id !=Null)
system.debug('case Record inserted successfully  ' + cs.Id);
