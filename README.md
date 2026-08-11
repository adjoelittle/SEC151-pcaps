# Sample Packet Captures — Classic Set

Practice capture files for SEC 151 (Protocol Analysis) labs. Open these in
**Wireshark** to practice filtering, protocol dissection, baselining, and
anomaly detection without needing to generate live traffic.

> **Looking for a specific lab's capture?** The required labs in Weeks 4, 5 and
> 7 use the purpose-built set in [`../pcaps-lab/`](../pcaps-lab/README.md), not
> the files here. Several captures in this classic set are only a handful of
> packets — perfect for illustrating one exchange, too small for the filtering
> and statistics work those labs ask for.

## Source & Attribution
These are the freely distributed companion capture files for **_Practical
Packet Analysis_ by Chris Sanders (No Starch Press)**. No Starch Press makes
the capture files available as a free public download to accompany the book.

- Book: https://nostarch.com/packetanalysis3
- Author: Chris Sanders — https://chrissanders.org

Please retain this attribution when redistributing.

## ⚠️ Usage Notes
- **Lab use only.** Analyze these captures in an isolated lab. Do not treat any
  address, host, or credential in them as live.
- **Some captures illustrate malicious or malformed traffic** (e.g.,
  `blaster.pcap`, `evilprogram.pcap`, `hauntedbrowser.pcap`, `dosattack.pcap`).
  These contain *packet data*, not executable files, but antivirus tools may
  still flag the traffic signatures. That is expected — they are teaching
  samples of what bad traffic looks like on the wire.

## Suggested mapping to course weeks
Captures **in bold** are the ones the lesson pages actually assign; the rest are
extra practice.

| Week | Focus | Example captures |
|------|-------|------------------|
| 2 | Journey of a packet | **`http.cap`** |
| 3 | Wireshark filtering & streams | **`http.cap`**, **`dns.cap`**, **`ftp.pcap`**, **`telnet.pcap`** |
| 4 | Ethernet / ARP / IP / ICMP | `arp.pcap`, `icmp.pcap`, `destunreachable.pcap`, `ipfragments.pcap` |
| 5 | TCP / UDP / DNS / DHCP / HTTP | **`dns.cap`**, **`http.cap`**, `dhcp.pcap`, `tcp-con-lost.pcap` |
| 6 | Baselining & performance | **`slowdownload.pcap`**, **`printerproblem.pcap`**, `torrential-slowness.pcap`, `icmp-tracert-slow.pcap` |
| 7 | Security analysis & anomalies | `portscan.pcap`, `osfingerprinting.pcap`, `blaster.pcap`, `evilprogram.pcap`, `covertinfo.pcap`, `hackersview.pcap` |

(Filenames reflect the classic Sanders companion set; assign whichever best fit
your lab prompts.)

## File formats
`.pcap`, `.cap`, and `.dmp` are all libpcap-family capture files and open
directly in Wireshark — no conversion needed.
