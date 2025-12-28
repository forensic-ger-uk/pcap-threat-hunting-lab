# pcap-threat-hunting-lab
Small lab to practise packet analysis and basic threat hunting in Wireshark

## Goals 
- Identify suspicious traffic patterns
- Document findings
- Build Timelines

## How to use
1. Open `pcaps/sample1.pcap` in Wireshark.
2. Apply filters such as `http`, `dns`, `tcp.flags.syn == 1 && tcp.flags.ack == 0`.
3. Note interesting hosts, URIs, and credentials in `analysis-notes/sample1-notes.md`.

## Tools used
- Wireshark

## Example findings
- Suspicious login attempts from a single IP over SSH.
- Cleartext credentials were visible in HTTP basic auth (lab data only).
