---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gtigrows.com
  spf: true
hosts:
- cert_expires: Aug 19 18:32:57 2026 GMT
  host: www.gtigrows.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Green Thumb Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Thumb Industries, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Green Thumb Industries
provider_slug: green-thumb-industries
slug: green-thumb-industries-domain-security
source_filename: green-thumb-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gtigrows.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 18:32:57 2026 GMT\n  hsts: false\ndomains:\n- domain: gtigrows.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-thumb-industries/refs/heads/main/security/green-thumb-industries-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cannabis
- Retail
- Consumer Products
- CPG
---
