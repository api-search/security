---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: infutor.com
  spf: true
hosts:
- cert_expires: Sep 23 20:48:04 2026 GMT
  host: infutor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infutor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infutor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Infutor
provider_slug: infutor
slug: infutor-domain-security
source_filename: infutor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infutor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 20:48:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: infutor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infutor/refs/heads/main/security/infutor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity Resolution
- Consumer Data
- Data Enrichment
- Lead Verification
- TCPA Compliance
- Marketing
- Identity
---
