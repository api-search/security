---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bloomscape.com
  spf: true
hosts:
- cert_expires: Sep 15 16:02:30 2026 GMT
  host: bloomscape.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloomscape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomscape, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bloomscape
provider_slug: bloomscape
slug: bloomscape-domain-security
source_filename: bloomscape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bloomscape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:02:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bloomscape.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomscape/refs/heads/main/security/bloomscape-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Houseplants
- E-Commerce
- Direct-to-Consumer
- Gardening
- Retail
---
