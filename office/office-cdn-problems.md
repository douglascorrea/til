## Problems with Office Cdn

I had problems to download Office 2016 for Mac OSX because the DNS was not resolving officecdn.microsoft.com.

After some search I found this [answer][http://answers.microsoft.com/en-us/office/forum/office_2016-office_install/office-2016-home-student-couldnt-install/8dbf4d0f-c69a-4e58-9afa-d062e1c59b43].

That guide me to put this line in `/etc/hosts`:

`193.77.14.147   officecdn.microsoft.com`

And it worked! (=
