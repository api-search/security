---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prized.dev
  spf: true
hosts:
- cert_expires: Sep 28 00:38:02 2026 GMT
  host: prized.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prized Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prized, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Prized
provider_slug: prized
slug: prized-domain-security
source_filename: prized-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prized.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 00:38:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: prized.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prized/refs/heads/main/security/prized-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Internal Tools
- AI
- Low-Code
- No-Code
- Automation
- Developer Tools
- Data Integration
- Security
- Audit
---
