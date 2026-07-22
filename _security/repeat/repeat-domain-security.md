---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getrepeat.io
  spf: true
hosts:
- cert_expires: Sep 29 18:04:28 2026 GMT
  host: getrepeat.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Repeat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Repeat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Repeat
provider_slug: repeat
slug: repeat-domain-security
source_filename: repeat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getrepeat.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:04:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getrepeat.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/repeat/refs/heads/main/security/repeat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Lifecycle Marketing
- Retention
- E-Commerce
- Customer Data
- Shopify
- CPG
---
