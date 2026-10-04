# RFC 1918

RFC 1918 is an IETF standard that reserves specific IPv4 address ranges for private local networks so they do not conflict with the public internet.

Reserved Private IP Ranges

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
    </ul>
  
  <h3 id="list-title">192.168.0.0-192.168.255.255 (192.168.0.0/16)</h3>
    <ul>
      <li>Size: 256 contiguous Class C networks (65,536 total addresses)</li>
      <li>Common use: Home Wi-Fi routers, small office/home office (SOHO) networks, and consumer gear.</li>
    </ul>
</ul>

<h2>References</h2>
<ul>
  <li>https://serverfault.com/questions/932626/why-do-people-use-172-x-x-x-instead-of-192-x-x-x</li>
  <li>https://www.arin.net/reference/research/statistics/address_filters/</li>
  <li>https://superuser.com/questions/369617/what-do-the-different-formats-for-network-addresses-indicate</li>
  <li>https://www.whatismyip.com/172-ip-address/</li>
</ul>
