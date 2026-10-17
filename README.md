# Networking Fundamentals & Traffic Analysis Notes (CYB 210)

**Status: Reference notes and planned packet-analysis exercises.** This repository currently contains study notes and exercise outlines, **not a completed PCAP/Zeek investigation**.

I originally started this repository while studying networking in SNHU's CYB 210. It is being retained as a place to practice protocol fundamentals and document future network investigations.

## What's here now

| Resource | Description | Status |
| --- | --- | --- |
| [OSI vs TCP/IP](./cheatsheets/osi-vs-tcpip.md) | Networking model reference | Written study notes |
| [Protocol basics](./cheatsheets/protocol-basics.md) | Common protocol and port reference | Written study notes |
| [Subnetting](./cheatsheets/subnetting.md) | CIDR and usable-host examples | Written study notes |
| [HTTP traffic analysis](./analysis-notes/http-traffic-analysis.md) | Steps for a future HTTP capture analysis | Planned exercise |
| [SYN flood analysis](./analysis-notes/syn-flood-analysis.md) | Steps for a future TCP SYN investigation | Planned exercise |

**Evidence status:** No usable packet-capture files or verified Zeek/Suricata results are currently published in this repository. Previous empty placeholder files are not valid captures.

## Future Lab Workflow

1. Capture or obtain traffic from a safe, authorized lab.
2. Record the environment, expected behavior, and test objective.
3. Inspect the trace with Wireshark; use Zeek only when actually installed and used.
4. Separate observations from hypotheses and link the relevant evidence.
5. Document findings, alternative explanations, and recommendations.

## Related Projects with Actual Evidence

- [SOC Incident Response Lab](https://github.com/Cspenc3/security-portfolio/tree/main/soc-incident-response-lab) — Wireshark screenshots and a documented DNS anomaly analysis.
- [CYB 220 Network Security Sandbox](https://github.com/Cspenc3/CYB220-project-one-sandbox) — network-security class lab documentation and screenshots.
- [Incident Response Workflows](https://github.com/Cspenc3/incident-response-workflows) — playbooks and example templates.

## Longer-Term Direction

Grow these notes into reproducible network-analysis exercises that support industrial network segmentation, firewall validation, and the future OT Security Architecture Lab.
