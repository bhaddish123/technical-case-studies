# Technical Case Studies

Formal write-ups referenced on my resume. This repository holds two PDFs — there is no application code here.

---

## Malware Traffic Analysis Using Wireshark

**File:** [Malware_Traffic_Analysis_using_Wireshark.pdf](Malware_Traffic_Analysis_using_Wireshark.pdf)

A PCAP-based network forensics investigation. I used Wireshark display filters to isolate HTTP, FTP, DNS, and TCP traffic, then looked for indicators of suspicious or automated client behavior and potential host compromise.

The write-up covers:

- Protocol-based filtering (DNS, FTP, HTTP, TCP) and address/field-based filters (`ip.addr`, `tcp.port`, Boolean operators)
- Web traffic analysis with `http.request`, including repeated connection attempts and abnormal retransmissions
- FTP analysis for a specific internal host (example filter in the PDF: `ftp && ip.addr == 192.168.3.10`)

---

## Ticket Verification System — UML & Use Cases

**File:** [Ticket_Verification_System_UML.pdf](Ticket_Verification_System_UML.pdf)

A systems-design case study for a ticket scanner that must stay consistent when train schedules change. The document works through use cases with a primary actor, main scenario, failure reasons, system responses, and alternative scenarios.

Cases in the write-up include:

1. The scanner updates the schedule (arrival and departure times), and flags mismatches for manual review.
2. If the schedule changes, the scanner assigns the passenger to the next valid train on the same route (including out-of-service-window and no-train-found outcomes).
3. The scanner confirms that an e-ticket's date and route match the current train, and rejects invalid tickets.

Class / use-case diagrams are in the PDF.

---

These are course / portfolio documents, not a running system.
