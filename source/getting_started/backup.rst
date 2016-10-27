*****************
Backup
*****************

|

It's always good to have a backup method in place.  Here are the steps to a basic backup method with FusionPBX. This is one of the many ways you can backup.

From the Gui.

**FreeSWITCH Source install paths.**

.. image:: ../_static/images/fusionpbx_backup_source1.jpg
        :scale: 85%



**FreeSWITCH Package install paths.**

.. image:: ../_static/images/fusionpbx_backup_source1.jpg
        :scale: 85%
        
::

 Goto Advanced > Default Settings.
 
 Settings for FreeSWITCH package installs are allready in place.
 
 For FreeSWITCH Source edit the backup paths
 path		array  	/usr/local/freeswitch/scripts 		True 	scripts  	 	
 path		array  	/usr/local/freeswitch/recordings 	True 	recordings  	
 path		array  	/var/www/fusionpbx 		        True 	fusionpbx  	
 path		array  	/usr/local/freeswitch/conf	        True 	conf  	
 path		array  	/usr/local/freeswitch/storage 		True 	storage
 
 Click "Reload" at the top of the page.


From the command line.

::
 
 
 cd /usr/src/fusionpbx-install.sh
 git pull
 cd debian/resources/backup/
 nano fusionpbx-backup.sh
 
 You will need to provide the database password
 Edit line #3 with the database passsword
 Save settings and exit
 
You should have the script ready to execute. (Default the script will use FreeSWITCH package paths.  If you have an older install using source be sure to change this by commenting the package line #22 and uncomment the source line #25.)
 
Setting crontab -e
 
::

 crontab -e
 Choose 1 for nano
 Goto the last blank line and paste in the next line.
 0 0 * * * bash /etc/cron.daily/fusionpbx-backup.sh
 press enter then save and exit.
 
 cd /usr/src/fusionpbx-install.sh/debian/resources/backup/
 cp fusionpbx-backup.sh /etc/cron.daily
 chmod 755 fusionpbx-backup.sh


Once this is complete you will have the backup ready to execute by ./fusion-backup.sh or from the daily cron job. From Advanced > Backup you can download the backup also. 

**FreeSWITCH Source install paths.**

.. image:: ../_static/images/fusionpbx_backup_source.jpg
        :scale: 85%


**FreeSWITCH Package install paths.**

.. image:: ../_static/images/fusionpbx_backup_package1.jpg
        :scale: 85%
