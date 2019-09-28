# Ping-in-CMD-Works-Well-While-Cannot-Open-any-Website-after-Cleaning-Trash
Yesterday after I cleaned trash with Huorong, I couldn't open any website with any explorer or use any program working with Internet，such as QQ.

Today I found that I could ping any website in CMD successfully. Now you can guess what goes wrong. Right! It must be something in the highest layer of TCP/IP protocol stack — the application layer. More specifically, it is the Winsock. "Winsock is a programming interface and the supporting program that handles input/output requests for Internet applications in a Windows operating system." — from Wikipedia.

I searched the Internet with my phone and found the solution here: http://www.itgemini.net/news/detail/3625.html. The solution is: type "netsh winsock reset" in the cmd with administrator privilege and restart your computer. Now try to open any website in your explorer — the feeling of going back to Internet is awesome!
