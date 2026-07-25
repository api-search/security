---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opengi.co.uk
  spf: true
hosts:
- cert_expires: Sep 29 15:30:26 2026 GMT
  host: www.opengi.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Gi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open GI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open GI
provider_slug: open-gi
slug: open-gi-domain-security
source_filename: open-gi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opengi.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:30:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opengi.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-gi/refs/heads/main/security/open-gi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Ireland
- Broker
- Agency Management
- Policy Administration
- Underwriting
- Insurtech
- Property and Casualty
- MGA
- Insurer Hosted Pricing
- Partner Gated
---
