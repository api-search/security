---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: muchbetteradventures.com
  spf: true
hosts:
- cert_expires: Sep 20 12:57:40 2026 GMT
  host: muchbetteradventures.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Much Better Adventures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Much Better Adventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Much Better Adventures
provider_slug: much-better-adventures
slug: much-better-adventures-domain-security
source_filename: much-better-adventures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: muchbetteradventures.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:57:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: muchbetteradventures.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/much-better-adventures/refs/heads/main/security/much-better-adventures-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Adventure Travel
- Tourism
- Booking
- Outdoor
- B Corp
---
