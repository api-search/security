---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gruve.ai
  spf: true
hosts:
- cert_expires: Sep 15 00:49:33 2026 GMT
  host: gruve.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gruve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gruve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gruve
provider_slug: gruve
slug: gruve-domain-security
source_filename: gruve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gruve.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:49:33 2026 GMT\n  hsts: false\ndomains:\n- domain: gruve.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gruve/refs/heads/main/security/gruve-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- AI Infrastructure
- Cybersecurity
- Security Operations
- Digital Forensics
- Data and AI
- Customer Experience
- Salesforce
- Enterprise Services
- Managed Services
---
