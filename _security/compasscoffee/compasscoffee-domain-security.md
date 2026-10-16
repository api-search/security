---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: compasscoffee.com
  spf: true
hosts:
- cert_expires: Nov 27 14:48:01 2026 GMT
  host: www.compasscoffee.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Compasscoffee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Compasscoffee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Compasscoffee
provider_slug: compasscoffee
slug: compasscoffee-domain-security
source_filename: compasscoffee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.compasscoffee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 14:48:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: compasscoffee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/compasscoffee/refs/heads/main/security/compasscoffee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Coffee
- Specialty
- Retail
- Subscription
- WashingtonDC
---
