**********
Features
**********

Adminer
---------

Integrated for an administrator in the superadmin group to enable easy database access.

Announcements
---------------

Setup a recording for the auto attendant that provides announcement to callers. (See `IVR Menus`_ )

Authentication
----------------

Web interface authentication by default authenticates against the FusionPBX Database. LDAP is one and has also been tested with Microsoft Active Directory an OpenLDAP.

Call Barge / Eavesdrop / Intercept
-----------------------------------


`Call Block`_
---------------

Block inbound calls by the caller id.

`Call Broadcast`_
-------------------

Create a recording and select one or more groups to have the system call and play the recording.

Call Center
------------

Creates a robust call center environment with agent tiers.

`Call Detail Records`_
------------------------

Various reporting capabilities to see who called, when, call length, export to a csv file, and call detail statistics.

`Call Flows`_ (Day Night Mode)
--------------------------------

Typically used with day night mode. To direct calls between two destinations. Can work with BLF on phone to show which direction call will be directed to.

`Call Forward`_
-----------------

Forward to another extension or to any phone number.

Call Monitoring
-----------------

View which extensions are currently in a call. (see `Active Extensions`_)

Call Pickup
-------------

For a particular extension or any extension that is currently ringing.

Call Queuing
--------------

Load calls into queues so they can be answered in the order they came into the queue. (see `Queues`_)

Call Recordings
-----------------

Record all or some calls or parts of the call. (See `Active Calls`_ and `Active Extensions`_)

Call Routing
--------------

Send the call different directions or perform actions based on reading the caller id info or other call information. (see `Dialplan Manager`_)

Call Announced Transfer
--------------------------------


Call Blind Transfer
---------------------------


Call Transfer
----------------------


Call Waiting
---------------------


Caller ID
------------------

Support for customization and supporting providers.

Conferencing
---------------------

Set up voice and video conference calls, is optionally secure with a PIN number, and can transfer current calls to a conference.  Interactive conference control provides ability to see the list of callers in the conference and manage the volume, see who is talking, kick, mute, unmute, deaf, undeaf, and more. (See `Conferences`_)

Conference Center
-------------------------

Unlimited conference rooms with moderator and paticipants, pin numbers, call recording, mute all, caller announce and more...

Configuration
---------------------

While the admin configures the system in the web interface. The data is saved to the database and can optionally be deliverd to FreeSWITCH via XML files, or on demand from the database.

`Contact Manager`_
--------------------------

Manage your contacts. Import contacts from Outlook CSV files. Export contacts to your cell phone with QR Codes. It is also possible to add additional features like time cards and invoices that can be related to the contacts.

Customizable
--------------------

FusionPBX has unprecedented customizability which can be used to meet your needs or the needs of your customers. Customizable themes, menu, dialplan, and more...

Dialplan
-----------

Dial by Name
--------------------

Search by first name or last name to find extension numbers on the system.

Direct Inward System Access (DISA)
-------------------------------------------

Gives ability to call into the system, put in a pin code, and then call back outbound.

Do Not Disturb (DND)
----------------------


Domain Based Multi-Tenant
--------------------------

Extensions
-----------


`Fax Server`_
----------------


Follow-Me
------------


Hot Desking
------------

A way to login to another phone device and temporarily or permanently become another extension. This is sometimes known as 'hoteling' and 'extension mobility'


Inbound and Outbound Call Routing
----------------------------------


`IVR Menus`_ (Auto Attendant)
------------------------------


Queues
--------


Music on Hold
--------------

Multi-Tenant
--------------------------------------------

domain based multi-tenant using subdomains such as red.pbxhosting.tld green.pbxhosting.tld blue.pbxhosting.tld

Operator Panel
---------------

Paging
--------


Parking
---------

Phone Setup and Provisioning
------------------------------


Provider Setup
----------------

Re-branding and Customize
--------------------------


`Recordings`_
----------------


`Ring Groups`_
-------------------



`Time Conditions`_
--------------------


User and Group Management
--------------------------


Voicemail
-----------

Has ability to copy voicemails for other voicemail boxes when receiving a voicemail. Additional features include voicemail to email and voicemail IVR.

Voicemail to Email
-------------------

Have voicemails sent to email.


.. _IVR Menus: /source/applications/ivr.rst
.. _Call Broadcast: Call_Broadcast
.. _Call Block: Call_Block
.. _Call Detail Records: Call_Detail_Records
.. _Call Forward: Call_Forward
.. _Call Flows: Call_Flows
.. _Contact Manager: Contact_Manager
.. _Dialplan Manager: http://docs.fusionpbx.com/en/latest/manual/dialplan.html?#dialplan-manager
.. _Active Extensions: Active_Extensions
.. _Queues: Queues
.. _Recordings: /source/applications/recordings.rst
.. _Call Recordings: /source/applications/recordings.rst
.. _Active Calls: Active_Calls
.. _Conferences: Conferences
.. _Fax Server: /source/applications/fax_server.rst
.. _Time Conditions: /source/applications/time_conditions.rst
.. _Ring Groups: /source/applications/ring_groups.rst
.. _Recordings: /source/applications/recordings.rst
.. _and lots more...: /source/features/features.rst
