---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: superbexperience.com
  spf: true
hosts:
- cert_expires: Aug 16 08:32:27 2026 GMT
  host: www.superbexperience.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 21:00:17 2026 GMT
  host: helpcenter.superbexperience.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superb Hq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superb, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Superb
provider_slug: superb-hq
slug: superb-hq-domain-security
source_filename: superb-hq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.superbexperience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 08:32:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: helpcenter.superbexperience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 21:00:17 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: superbexperience.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superb-hq/refs/heads/main/security/superb-hq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurants
- Reservations
- Hospitality
- Guest Experience
- GXM
- Point of Sale
- CRM
- Payments
---
