---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chipotle.com
  spf: true
hosts:
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: www.chipotle.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chipotle Mexican Grill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chipotle Mexican Grill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chipotle Mexican Grill
provider_slug: chipotle-mexican-grill
slug: chipotle-mexican-grill-domain-security
source_filename: chipotle-mexican-grill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chipotle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: chipotle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chipotle-mexican-grill/refs/heads/main/security/chipotle-mexican-grill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Burritos
- Catering
- Digital Ordering
- Fast Casual
- Food Safety
- Fortune 500
- Loyalty
- Mobile App
- Quick Service Restaurant
- Restaurant Technology
- Restaurants
- Rewards
---
