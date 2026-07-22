---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rohirrim.ai
  spf: true
hosts:
- cert_expires: Aug 24 20:58:16 2026 GMT
  host: rohirrim.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rohirrim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rohirrim, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rohirrim
provider_slug: rohirrim
slug: rohirrim-domain-security
source_filename: rohirrim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rohirrim.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 20:58:16 2026 GMT\n  hsts: false\ndomains:\n- domain: rohirrim.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rohirrim/refs/heads/main/security/rohirrim-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Ml
- Government
- Procurement
- Acquisition
- Proposals
- RFP
- GovTech
- Artificial Intelligence
---
