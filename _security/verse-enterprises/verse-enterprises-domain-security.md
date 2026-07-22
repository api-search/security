---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: verse.inc
  spf: true
hosts:
- cert_expires: Aug  1 12:32:32 2026 GMT
  host: verse.inc
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verse Enterprises Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verse Enterprises, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Verse Enterprises
provider_slug: verse-enterprises
slug: verse-enterprises-domain-security
source_filename: verse-enterprises-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verse.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 12:32:32 2026 GMT\n  hsts: false\ndomains:\n- domain: verse.inc\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verse-enterprises/refs/heads/main/security/verse-enterprises-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Energy
- Clean Energy
- Climate
- Artificial Intelligence
- Energy Management
- Sustainability
- SaaS
---
