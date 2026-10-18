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

<h2>A & AAAA Records (Forward Lookups)</h2>
  <p>These are the foundational blocks of the internet. When you type a website URL into a browser, your system queries <b>A records</b> for IPv4 networks or AAAA records for IPv6 networks to locate the hosting server.</p>

<h2>PTR Records (Reverse Lookups)</h2>
  <p>Unlike A and AAAA records a <b>PTR record</b> starts with the IP address and looks up the associated domain name. It is configured inside a special top level routing domain called .arpa</p>
    <ul>
      <li>Common Use Case: Mostly utilized by emall servers to verify the sender's identity. It a mail server claims to be from company.com but its IP address's PTR record points somewhere else, receiving servers will            likely flag the email as spam.</li>
    </ul>

<h2>HTTPS Records (Service Binding)</h2>
  <p>The <b>HTTPS record</b> is a newer, highly specialized record type. Historically, when a browser visited a sile, it had to connect via standard HTTP first, get a redirect to HTTPS, and then negotiate secure protocols.    </p>
    <ul>
      <li>The HTTPS record allows the authoritative DNS server to tell the browser exactly how to securely connect right away including which HTTP versions are supported (like HI IP/3) and public key components for               Encrypted Client Hello (ECH)-improving both speed and privacy.</li>
    </ul>
