---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eve.legal
  spf: true
hosts:
- cert_expires: Aug 16 17:46:44 2026 GMT
  host: www.eve.legal
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eve Legal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eve
provider_slug: eve-legal
slug: eve-legal-domain-security
source_filename: eve-legal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eve.legal\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 17:46:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eve.legal\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eve-legal/refs/heads/main/security/eve-legal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal AI
- Legal Technology
- Plaintiff Law
- Personal Injury
- Labor And Employment
- Case Intake
- Demand Letters
- Medical Chronology
- Discovery
- Litigation
- Document Drafting
- AI Agents
- Voice Agent
- Case Auditing
- SaaS
- SOC 2
- HIPAA
- Butler Labs
---
