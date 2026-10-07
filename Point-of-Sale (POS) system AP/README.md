# Point-of-Sale (POS) system Access Point (AP)
As I was browsing on the platform Reddit, I stumbled across some post that have two Ubiquiti Access Point (AP) that are right next to each other, which made me quesiton, why? And I seem to notice it too in some malls that I've visit.

<h2>What is Point-of-Sale (POS)?</h2>
<p>POS stands for Point of Sale. It refers to connecting, prioritizing, or segmenting wireless or wired traffic for digital cash registers, card payment terminals, and inventory scanners.</p>
<ul>
  <li>Network Segmentation (VLANs): Business networks often use Virtual Local Area Networks (VLANs) to separate POS hardware from public guest Wi-Fi. This keeps sensitive payment and customer data secure from outside           users.</li>
  <li>Traffic Prioritization (QoS): Access points often feature Quality of Service (QoS) rules to ensure that payment transactions take priority over general web browsing or customer streaming. This prevents slow credit card   approvals during busy hours.</li>
  <li>Dedicated SSIDs: Network administrators frequently configure a hidden or private Wi-Fi name (SSID) on the access point exclusively for the store's POS tablets and barcode scanners.</li>
  <li>Firewall Protection: Block unauthorized inbound and outbound traffic to the POS subnet.</li>
  <li>Access Control: Disable SSID broadcasting and limit connections to authorized MAC addresses.</li>
</ul>

<h2>PCI Compliance?</h2>
<p>PCI compliance for a wireless Point-of-Sale (POS) device connected through a Wi-Fi access point means ensuring that the wireless network infrastructure securely transmits payment data without exposing it to unauthorized users.</p>
<ul>
  <li>Network Segmentation (VLANs): Business networks often use Virtual Local Area Networks (VLANs) to separate POS hardware from public guest Wi-Fi. This keeps sensitive payment and customer data secure from outside           users.</li>
  <li>Traffic Prioritization (QoS): Access points often feature Quality of Service (QoS) rules to ensure that payment transactions take priority over general web browsing or customer streaming. This prevents slow credit card   approvals during busy hours.</li>
  <li>Dedicated SSIDs: Network administrators frequently configure a hidden or private Wi-Fi name (SSID) on the access point exclusively for the store's POS tablets and barcode scanners.</li>
  <li>Firewall Protection: Block unauthorized inbound and outbound traffic to the POS subnet.</li>
</ul>

<h2> Implementation Options</h2>
<table border="1" style="border-collapse: collapse; width: 100%; text-align: left;">
  <thead>
    <tr>
      <th>Strategy</th>
      <th>Pros</th>
      <th>Cons</th>
      <th>Best For</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Physical AP Separation</td>
      <td>Easiest to audit and verify visually</td>
      <td>Requires buying extra hardware</td>
      <td>Small shops with basic setups</td>
    </tr>
    <tr>
      <td>VLAN Segmentation</td>
      <td>Uses existing hardware efficiently</td>
      <td>Complex configuration prone to errors</td>
      <td>Locations with IT support</td>
    </tr>
  </tbody>
</table>

<h2>References</h2>
<ul>
  <li>https://listings.pcisecuritystandards.org/pdfs/PCI_DSS_v2_Wireless_Guidelines.pdf</li>
  <li>https://www.youtube.com/watch?v=N-qQwslLoP0&t=20</li>
  <li>https://pcidssguide.com/pci-dss-rogue-wireless-access-point-protection/</li>
  <li>https://www.fortinet.com/resources/cyberglossary/what-is-pci-compliance</li>
  <li>https://kirkpatrickprice.com/video/pci-requirement-9-1-3-restrict-physical-access-wireless-access-points-gateways-handheld-devices-networking-communications-hardware-telecommunication-lines/</li>
  <li>https://www.reddit.com/r/Ubiquiti/comments/r563op/tell_me_you_dont_understand_wifi_gear_without/</li>
  <li>https://www.itretail.com/blog/pos-pci-compliance</li>
  <li>https://squareup.com/ca/en/the-bottom-line/operating-your-business/pci-compliance</li>
  <li>https://www.reddit.com/r/networking/comments/nyh45b/point_of_sale_networking_general_advice_inquiry/</li>
  <li>https://www.quora.com/How-does-a-point-of-sale-system-PoS-work-using-WiFi</li>
  <li>https://www.technibble.com/forums/threads/adding-wireless-access-to-one-room.46834/</li>
  <li>https://www.tp-link.com/ph/blog/2512/setting-up-wi-fi-for-your-small-business-in-the-philippines-cafes-salons-and-spas/</li>
  <li>https://listings.pcisecuritystandards.org/documents/PCI_DSS-QRG-v3_2_1.pdf</li>
  <li>https://www.reddit.com/r/Ubiquiti/comments/y4to4x/spotted_in_the_wild/</li>
  <li>https://www.reddit.com/r/Ubiquiti/comments/1lq34qr/spotted_in_the_wild/</li>
  <li>https://www.reddit.com/r/Ubiquiti/comments/1bfs61r/caught_in_the_wild/</li>
  <li>https://www.reddit.com/r/Ubiquiti/comments/1qxq1ui/spotted_in_the_wild_2_is_better_than_1/</li
</ul>
