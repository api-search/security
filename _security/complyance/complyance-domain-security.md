---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: complyance.com
  spf: true
hosts:
- cert_expires: Oct  4 04:30:02 2026 GMT
  host: www.complyance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Complyance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Complyance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Complyance
provider_slug: complyance
slug: complyance-domain-security
source_filename: complyance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.complyance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 04:30:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: complyance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/complyance/refs/heads/main/security/complyance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Governance Risk Compliance
- GRC
- Compliance
- Risk Management
- Security
- Vendor Management
- Audit
- Policy Management
---
