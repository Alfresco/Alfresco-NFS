Alfresco NFS
=======
In alfresco 5.1 the NFS code has reached End Of Life, EOL.

This project contains the code before removal from the 
main alfresco code base and may be used to form a community led module 
to add back NFS functionality to alfresco.   

The code in this project corresponds to revision r109179 in Alfresco's SVN repository.

Interested parties should contact Alfresco to collaborate with this project.
Best way to contact us is to email community@alfresco.com

If we get a lot of interest in the module, then we can prioritize building necessary extension points as a future activity.

Overview
-------
For the End of life for NFS the mapping between the spring configuration for NFS and LJAN was removed.   The JLAN interface remains unchanged.
There are 11 files affected.  3 of which have simply been deleted.   Which are enclosed here.   2 which have code removed,  these are the problem files.  
And configuration files which have had NFS configuration stripped from them,  these are enclosed as deltas to the existing file.

Next Steps
-------
The code will not work without a little rework in particular 
* The code needs packaging somehow either into a module or other delivery package.
* The ServerConfigurationBean (and the abstract base) needs rework to enable it to be modified and extended.
* The alfresco spring configuration needs to be reworked such that the NFS context can be injected cleanly.
* The old code needs to be integrated with alfresco itself.




