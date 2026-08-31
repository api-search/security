---
certifications:
- SOC 2 Type 2
- PCI DSS v4.0.1
description: Too Good To Go runs a hosted SafeBase trust center at trust.toogoodtogo.com covering product security, data security, access control, infrastructure, endpoint security, incident response, risk management, business continuity / disaster recovery, employee training and continuous monitoring. Reports are listed as gated downloads (NDA/request flow) rather than public PDFs; the certifications themselves are stated publicly. The host answers 403 to plain HTTP clients (Cloudflare bot challenge) and renders for a browser, so the 403 below is an edge policy, not an absent page.
kind: trust-center
layout: security
name: Too Good To Go Trust Center
name_suffix: Trust Center
overview: Too Good To Go maintains a public trust center documenting SOC 2 Type 2 and PCI DSS v4.0.1 compliance.
provider_name: Too Good To Go
provider_slug: too-good-to-go
slug: too-good-to-go-trust-center
source_filename: too-good-to-go-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nprobe: true\nsource: https://trust.toogoodtogo.com/\nurl: https://trust.toogoodtogo.com/\nname: Too Good To Go Trust Center\nplatform: SafeBase (toogoodtogo.portals.safebase.io)\ndescription: >-\n  Too Good To Go runs a hosted SafeBase trust center at trust.toogoodtogo.com covering\n  product security, data security, access control, infrastructure, endpoint security,\n  incident response, risk management, business continuity / disaster recovery, employee\n  training and continuous monitoring. Reports are listed as gated downloads (NDA/request\n  flow) rather than public PDFs; the certifications themselves are stated publicly.\n  The host answers 403 to plain HTTP clients (Cloudflare bot challenge) and renders for a\n  browser, so the 403 below is an edge policy, not an absent page.\ncertifications:\n- name: SOC 2 Type 2\n  status: certified\n  evidence: https://trust.toogoodtogo.com/\n- name: PCI DSS v4.0.1\n  status: certified\n \
  \ evidence: https://trust.toogoodtogo.com/\ndocuments:\n- name: SOC 2 Report\n  access: gated\n- name: PCI DSS Report\n  access: gated\n- name: Pentest Report\n  access: gated\nauditor_named: Deloitte\nevidence:\n- source: https://trust.toogoodtogo.com/\n  http_status: 403\n  note: >-\n    403 to curl with a browser User-Agent (Cloudflare challenge); content read via a\n    rendering fetch on 2026-08-30, which returned the trust-center copy and the two\n    certification names above.\n  keywords:\n  - soc 2 type 2\n  - pci dss v4.0.1\n  - pentest report\n  - trust center\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/too-good-to-go/refs/heads/main/security/too-good-to-go-trust-center.yml
summary_line: SOC 2 Type 2, PCI DSS v4.0.1
tags:
- Company
- Food Waste
- Surplus Food
- Marketplace
- Sustainability
- Grocery Retail
- Consumer App
- Climate Tech
- B Corporation
- Denmark
trust_url: https://trust.toogoodtogo.com/
---
