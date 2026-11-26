# Mission 7: Networking

## 1. Mission Title
Networking Basics

## 2. Task/Objective
Practise using basic networking commands to see how my laptop connects to a network and communicates with other machines online.

## 3. Work Completed
- Checked my Mac's local IP addresses using `ifconfig`.
- Pinged `google.com` to test connectivity and measure the round-trip response time.
- Used `nslookup` to resolve `google.com` from a domain name into an IP address.
- Ran `traceroute` to see the path and router hops my data takes to reach Google's servers.

## 4. Commands/Tools Used
`ifconfig | grep "inet "`, `ping -c 4 google.com`, `nslookup google.com`, `traceroute google.com`

## 5. My Understanding
An IP address is basically a unique numeric label that identifies a device on a network so data knows where to go. When I ran `ping`, it sent small test packets to `google.com` to check if the server was reachable and measured the latency in milliseconds. Humans remember names much easier than long numbers, so DNS (which I checked with `nslookup`) translates a readable domain name like `google.com` into the actual IP address my computer connects to. Finally, `traceroute` shows every router, or "hop," that my packets pass through on their way to the destination server.

## 6. Difficulties Faced
Some routers don't reply to trace probes, so `traceroute` started printing `* * *` timeouts on later hops and took a while to finish.

## 7. How I Resolved Them
Once I had plenty of hops printed out to show the route, I pressed `Ctrl+C` to stop the command cleanly.

## 8. Evidence/Files
Terminal output showing `ifconfig`, `ping`, `nslookup`, and `traceroute` results (see commit history and screenshots).