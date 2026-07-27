---
certifications:
- PCI DSS
- ISO/IEC 27001
- NIST CSF
- SOC 1 Type 2
- SOC 1 Type 2
description: ''
kind: trust-center
layout: security
name: Homes Com Trust Center
name_suffix: Trust Center
overview: Homes.com maintains a public trust center documenting PCI DSS, ISO/IEC 27001, NIST CSF, SOC 1 Type 2, and SOC 1 Type 2 compliance.
provider_name: Homes.com
provider_slug: homes-com
slug: homes-com-trust-center
source_filename: homes-com-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nprobe: true\nsource: https://trust.costargroup.com/\nurl: https://trust.costargroup.com/\nscope: parent-company\nscope_note: >-\n  Homes.com publishes no trust center of its own — trust.homes.com is NXDOMAIN\n  and every path on www.homes.com returns HTTP 403 to non-browser clients behind\n  Akamai bot protection. The trust center recorded here belongs to CoStar Group,\n  Inc., the company that owns and operates Homes.com (acquired 2021, Homesnap\n  folded in). It is the corporate security posture that governs the Homes.com\n  property, but the portal does NOT name Homes.com, Apartments.com, Homesnap, or\n  LoopNet in its covered-product list; the only products named explicitly are\n  Visual Lease and CoStar Real Estate Manager. Read the certifications below as\n  CoStar Group corporate scope, not as a Homes.com-specific attestation.\nplatform: SafeBase\nplatform_evidence:\n  dns_cname: costargroup.portals.safebase.io\n  note: >-\n\
  \    trust.costargroup.com is a CNAME to costargroup.portals.safebase.io — a\n    SafeBase-hosted trust portal. The host is fronted by Cloudflare and returns\n    HTTP 403 with a managed browser challenge to curl; content below was read\n    through a rendering fetch.\ncertifications:\n  - name: PCI DSS\n    scope: CoStar Group\n  - name: ISO/IEC 27001\n    scope: CoStar Group\n  - name: NIST CSF\n    scope: CoStar Group\n    note: Framework alignment, listed alongside the certifications on the portal.\n  - name: SOC 1 Type 2\n    scope: Visual Lease\n    period: 'November 1, 2025 to April 30, 2026'\n    verbatim: >-\n      Visual Lease SOC 1 Type 2 attestation report for the examination period\n      from November 1, 2025 to April 30, 2026\n  - name: SOC 1 Type 2\n    scope: CoStar Real Estate Manager\n    period: 'April 1, 2025 to March 31, 2026'\n    verbatim: >-\n      CoStar Real Estate Manager's SOC 1 Type 2 attestation report for the\n      examination period from April 1, 2025\
  \ to March 31, 2026\nnot_found:\n  - SOC 2\n  - HIPAA\n  - FedRAMP\n  - CSA STAR\n  - subprocessor list\ncontacts:\n  security: costarsecurity1@costar.com\n  vulnerability_disclosure: csgpappsec@costar.com\ndocument_access: >-\n  Attestation reports are listed on the portal; SafeBase gates document download\n  behind an NDA/request flow. No report was downloaded.\nevidence:\n  - source: https://trust.costargroup.com/\n    status: 403\n    note: >-\n      403 to curl (Cloudflare managed challenge); content read via rendering\n      fetch on 2026-07-26.\n    keywords: [pci dss, iso/iec 27001, nist csf, soc 1 type 2, trust center]\n  - source: dig CNAME trust.costargroup.com\n    result: costargroup.portals.safebase.io\n    kind: dns\nprobes:\n  - url: https://trust.homes.com/\n    status: 000\n    note: DNS NXDOMAIN — Homes.com publishes no trust center subdomain.\n  - url: https://trust.costargroup.com/\n    status: 403\n  - url: https://security.costargroup.com/\n    status: 000\n    note:\
  \ DNS NXDOMAIN.\n  - url: https://trust.costargroup.com/.well-known/security.txt\n    status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homes-com/refs/heads/main/security/homes-com-trust-center.yml
summary_line: PCI DSS, ISO/IEC 27001, NIST CSF, SOC 1 Type 2, SOC 1 Type 2
tags:
- Real Estate
- United States
- Property Listings
- MLS
- RESO
- IDX
- Rentals
- PropTech
- Portals
- Marketplaces
- Residential Real Estate
- Real Estate Agents
- Brokers
- Listings Syndication
- CoStar Group
trust_url: https://trust.costargroup.com/
---
