# Common Subnet Masks
There are many other IPv4 subnet masks besides 255.255.255.0 (often written shorthand as 255.255.255). 
A subnet mask is 32 bits long, divided into four octets, and each subnet mask sets how many IP addresses are in a network and how many devices (hosts) can connect to it.

<h2>Common Subnet Masks</h2>
<ul>
  <li>255.0.0.0 (/8): Allows up to 16,777,214 usable host addresses (often used in large networks or default Class A ranges).</li>
  <li>255.255.0.0 (/16): Allows up to 65,534 usable host addresses (common in larger enterprise or campus networks).</li>
  <li>255.255.254.0 (/23): Allows up to 510 usable host addresses (combines two /24 blocks).</li>
  <li>255.255.255.0 (/24): Allows up to 254 usable host addresses (the standard for most home and small office networks).</li>
  <li>255.255.255.128 (/25): Allows up to 126 usable host addresses (splits a /24 in half).</li>
  <li>255.255.255.192 (/26): Allows up to 62 usable host addresses.</li>
  <li>255.255.255.224 (/27): Allows up to 30 usable host addresses.</li>
  <li>255.255.255.240 (/28): Allows up to 14 usable host addresses.</li>
  <li>255.255.255.248 (/29): Allows up to 6 usable host addresses.</li>
  <li>255.255.255.252 (/30): Allows up to 2 usable host addresses (traditionally used for point-to-point router links).</li>
  <li>255.255.255.254 (/31): Used for point-to-point links with 2 addresses and no separate network/broadcast overhead.</li>
  <li>255.255.255.255 (/32): Targets a single host IP address.
</ul>

<h2>Things to Keep in Mind</h2>
<ul>
  <li>CIDR Notation: Network engineers often write /24, /16, or /30 instead of typing out the full four-part mask. 
    You can explore a full breakdown of prefixes and host counts in the <a href="https://www.freecodecamp.org/news/subnet-cheat-sheet-24-subnet-mask-30-26-27-29-and-other-ip-address-cidr-network-references/">freeCodeCamp Subnet Cheat Sheet</a>.
 </li>
  <li>Consistency on a Network: Most users on <a href="https://www.reddit.com/r/HomeNetworking/comments/zpiyeb/what_is_the_difference_between_subnet_masks/)">Reddit's r/HomeNetworking</a> agree that mismatched subnet masks across devices on the same local network can cause connectivity problems. 
    Likewise, most users on <a href="https://networkengineering.stackexchange.com/questions/25952/is-there-a-downside-to-using-a-subnet-mask-other-than-255-255-255-0">Network Engineering Stack Exchange</a> agree that using broader masks like 255.0.0.0 on private LANs requires care to avoid unintended IP range conflicts.</li>
</ul>

<h2>References</h2>
<ul>
  <li>https://networkengineering.stackexchange.com/questions/25952/is-there-a-downside-to-using-a-subnet-mask-other-than-255-255-255-0</li>
  <li>https://www.freecodecamp.org/news/subnet-cheat-sheet-24-subnet-mask-30-26-27-29-and-other-ip-address-cidr-network-references/</li>
  <li>https://www.reddit.com/r/HomeNetworking/comments/zpiyeb/what_is_the_difference_between_subnet_masks/</li>
  <li>https://www.ipxo.com/subnet-cheat-sheet/</li>
  <li>https://learn.microsoft.com/en-us/troubleshoot/windows-client/networking/tcpip-addressing-and-subnetting</li>
  <li>https://www.cisco.com/c/en/us/support/docs/ip/routing-information-protocol-rip/13788-3.html</li>
</ul>
