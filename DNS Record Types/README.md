# DNS Record Types
DNS Record Type (Pi-hole)

<h2>What is DNS Record Types?</h2>
  <p>DNS resource records map human-readable domain names to machine-readable data, each serving a specific routing or security purpose</p>
    <table>
  <thead>
    <tr>
      <th>Query Type</th>
      <th>Full Name</th>
      <th>Primary Purpose</th>
      <th>Example Mapping</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>A</td>
      <td>Address Record</td>
      <td>Maps a domain name to a 32-bit IPv4 address</td>
      <td>example.com &rarr; 102.0.2.1</td>
    </tr>
    <tr>
      <td>AAAA</td>
      <td>Quad-A Record</td>
      <td>Maps a domain name to a 128-bit IPv6 address</td>
      <td>example.com &rarr; 2001:db8::1</td>
    </tr>
    <tr>
      <td>PTR</td>
      <td>Pointer Record</td>
      <td>Performs a reverse DNS lookup (IP to domain)</td>
      <td>1.2.0.102.in-addr.arpa &rarr; example.com</td>
    </tr>
    <tr>
      <td>HTTPS</td>
      <td>HTTPS Binding Record</td>
      <td>Provides connection parameters and encryption keys before connection</td>
      <td>Reduces overhead by avoiding unencrypted HTTP redirects</td>
    </tr>
  </tbody>
</table>
