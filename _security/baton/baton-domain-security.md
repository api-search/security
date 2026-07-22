---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: baton.io
  spf: true
hosts:
- cert_expires: Sep 27 18:54:43 2026 GMT
  host: baton.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Baton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baton, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Baton
provider_slug: baton
slug: baton-domain-security
source_filename: baton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: baton.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 18:54:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: baton.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baton/refs/heads/main/security/baton-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Supply Chain
- Freight
- Transportation
- Visibility
---
