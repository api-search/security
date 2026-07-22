---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: snoutid.com
  spf: true
hosts:
- cert_expires: Sep 13 00:11:21 2026 GMT
  host: snoutid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Snout
provider_slug: snout
slug: snout-domain-security
source_filename: snout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snoutid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 00:11:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: snoutid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snout/refs/heads/main/security/snout-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Veterinary
- Pet Care
- Wellness Plans
- Subscription
- Payments
- Healthcare
---
