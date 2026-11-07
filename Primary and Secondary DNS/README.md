# Primary and Secondary DNS
Primary and secondary DNS servers work together as a master-and-copy system to translate domain names into IP addresses while ensuring your website stays online.

<h2>How the Primary DNS Works</h2>
<ul>
  <li>Source of Truth: The Primary DNS server holds the master, read-write copy of a domain's zone file (which contains all records like A, AAAA, MX, and CNAME).</li>
  <li>Admin Control: Administrators make all changes—such as adding a new subdomain or updating an IP address—directly on this primary server.</li>
  <li>Start of Authority (SOA): It tracks changes using an SOA serial number.</li>
</ul>

<h2>How the Secondary DNS Works</h2>
<ul>
  <li>Read-Only Copy: The Secondary DNS server holds an identical, read-only copy of the domain's zone file.</li>
  <li>Zone Transfers: It stays synchronized through automated updates called zone transfers (using protocols like AXFR or IXFR) whenever the primary server changes its serial number.</li>
  <li>Failover & Redundancy: If the primary server crashes, goes offline, or experiences a network outage, the secondary server steps in seamlessly to answer DNS queries without dropping user traffic.
  </li>
  <li>Load Balancing: Both servers can actively respond to queries, sharing the workload and providing faster response times depending on user location.</li>
</ul>

<h2>References</h2>
<ul>
  <li>https://www.youtube.com/watch?v=qhiyTH5B21A&t=63s</li>
  <li>https://www.youtube.com/watch?v=kiVIaQF_3Yc</li>
  <li>https://www.ibm.com/think/topics/primary-vs-secondary-dns</li>
  
</ul>
