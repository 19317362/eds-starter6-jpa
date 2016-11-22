Online Demo: https://demo.rasc.ch/eds-starter6/

Logins

| Email             | Password  |
| ----------------- |---------- |
| admin@starter.com | admin     |
| user@starter.com  | user      |

If Eclipse gives error on "The Maven APT plugin has a known issue that prevents its usage directly from Eclipse..."

SOLUTION 1

Following this link


"The Maven APT plugin has a known issue that prevents its usage directly from Eclipse. Eclipse users must create the Querydsl query types manually by running the command mvn generate-sources at command prompt."

So i execute the command line mvn generate-sources in my project floder with console cmd and i got my Qclasses generated.

SOLUTION 2 from @informatik01 comment

we can explicitly specified JVM in the eclipse.ini like that :
-vm
path\to\javaw.exe
 -vmargs...
The -vm option must occur before the -vmargs option and for more info read @informatik01 comment below.

