# RFC 1918

RFC 1918 is an IETF standard that reserves specific IPv4 address ranges for private local networks so they do not conflict with the public internet.
Reserved Private IP Ranges
<ul>
  <li>10.0.0.0 – 10.255.255.255 (10/8 prefix / Single Class A)</li>
  <li>172.16.0.0 – 172.31.255.255 (172.16/12 prefix / 16 contiguous Class B blocks)</li>
  <li>192.168.0.0 – 192.168.255.255 (192.168/16 prefix / 256 contiguous Class C blocks)</li>
</ul>




192.168.0.0-192.168.255.255 (192.168.0.0/16)
Size: 256 contiguous Class C networks (65,536 total addresses)
Common use: Home Wi-Fi routers, small office/home office (SOHO) networks, and consumer gear. Super User 3

<h2>The Three RFC 1918 Private Address Ranges</h2>
<ul>
  <h3 id="list-title">10.0.0.0 – 10.255.255.255 (10/8 prefix / Single Class A)</h3>
    <ul>
      <li>Size: Single Class A network (16,777,216 total addresses)</li>
      <li>Common use: Very large enterprise networks, corporate campuses, and cloud infrastructure (like AWS or GCP VPCS)</li>
    </ul>

  <h3 id="list-title">172.16.0.0-172.31.255.255 (172.16.0.0/12)</h3>
    <ul>
      <li>Size: 16 contiguous Class B networks (1,048,576 total addresses)</li>
      <li>Common use: Medium-to-large corporate networks, universities, Docker containers, and mobile networks.</li>
      <li>Important note: Only the 172.16.x.x through 172.31.x.x block is private; any other 172.x.x.x address is a publicly routable internet
address. </li>
      <li><a href="https://pearos.xyz/nicecore/">PearOS</a></li>
    </ul>
  
  <h3 id="list-title">Server</h3>
    <ul>
      <li><a href="https://www.debian.org/distrib/">Debian</a></li>
      <li><a href="https://fedoraproject.org/server/download/">Fedora</a></li>
      <li><a href="https://ubuntu.com/download/server">Ubuntu Server</a></li>
      <li><a href="https://www.zimaspace.com/zimaos/download">ZimaOS</a></li>
    </ul>
</ul>
