# Primary and Secondary DNS
Primary and secondary DNS servers work together as a master-and-copy system to translate domain names into IP addresses while ensuring your website stays online.

<h2>How the Primary DNS Works</h2>
<ul>
  <li><b>Source of Truth:</b> The Primary DNS server holds the master, read-write copy of a domain's zone file (which contains all records like A, AAAA, MX, and CNAME).</li>
  <li><b>Admin Control:</b> Administrators make all changes, such as adding a new subdomain or updating an IP address directly on this primary server.</li>
  <li><b>Start of Authority (SOA):</b> It tracks changes using an SOA serial number.</li>
</ul>

<h2>How the Secondary DNS Works</h2>
<ul>
  <li><b>Read-Only Copy:</b> The Secondary DNS server holds an identical, read-only copy of the domain's zone file.</li>
  <li><b>Zone Transfers:</b> It stays synchronized through automated updates called zone transfers (using protocols like AXFR or IXFR) whenever the primary server changes its serial number.</li>
  <li><b>Failover & Redundancy:</b> If the primary server crashes, goes offline, or experiences a network outage, the secondary server steps in seamlessly to answer DNS queries without dropping user traffic.
  </li>
  <li><b>Load Balancing:</b> Both servers can actively respond to queries, sharing the workload and providing faster response times depending on user location.</li>
</ul>

<h2>Note</h2>
<p>
  Note: On client devices or home routers, operating systems may query servers in different ways rather than sticking strictly to a rigid "primary then secondary" sequence, though opinions on client behavior differ across platforms such as Reddit.
</p>

<h2>References</h2>
<ul>
  <li>https://www.youtube.com/watch?v=qhiyTH5B21A&t=63s</li>
  <li>https://www.youtube.com/watch?v=kiVIaQF_3Yc</li>
  <li>https://www.ibm.com/think/topics/primary-vs-secondary-dns</li>
  <li>https://www.cloudflare.com/learning/dns/glossary/primary-secondary-dns/</li>
  <li>https://learn.microsoft.com/en-us/answers/questions/621888/primary-and-secondary-dns-working</li>
  <li>https://leasepacket.com/primary-vs-secondary-dns-servers/</li>
  <li>https://www.cloudns.net/blog/master-slave-dns/</li>
  <li>https://www.youtube.com/watch?v=-iQ4XvfkJ10</li>
  <li>https://www.digicert.com/blog/what-is-primary-dns</li>
  <li>https://www.youtube.com/shorts/913tWov7gvU</li>
  <li>https://www.reddit.com/r/HomeNetworking/comments/18acmex/how_does_typical_home_wifi_routers_use_primary/</li>
</ul>
