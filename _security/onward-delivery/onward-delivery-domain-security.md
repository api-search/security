---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: onwarddelivery.com
  spf: true
hosts:
- cert_expires: Sep 27 08:21:48 2026 GMT
  host: onwarddelivery.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 12:19:37 2026 GMT
  host: docs.onwarddelivery.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 04:35:00 2026 GMT
  host: api.onwarddelivery.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onward Delivery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onward Delivery, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Onward Delivery
provider_slug: onward-delivery
slug: onward-delivery-domain-security
source_filename: onward-delivery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onwarddelivery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 08:21:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.onwarddelivery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:19:37 2026 GMT\n  hsts: null\n- host: api.onwarddelivery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:35:00 2026 GMT\n  hsts: null\ndomains:\n- domain: onwarddelivery.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onward-delivery/refs/heads/main/security/onward-delivery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Final Mile
- Last Mile Delivery
- Freight
- Shipping
- Transportation
- Supply Chain
- Carriers
---
