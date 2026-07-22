---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rebookify.com
  spf: true
hosts:
- cert_expires: Sep 15 16:32:38 2026 GMT
  host: rebookify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rebookify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rebookify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rebookify
provider_slug: rebookify
slug: rebookify-domain-security
source_filename: rebookify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rebookify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:32:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rebookify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rebookify/refs/heads/main/security/rebookify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Hospitality
- Hotels
- Booking
- Price Monitoring
- Travel Technology
---
