---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: postmates.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uber.com
  spf: true
hosts:
- cert_expires: Aug 27 02:27:14 2026 GMT
  host: postmates.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: developer.uber.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 02:27:14 2026 GMT
  host: api.postmates.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Postmates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Postmates, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Postmates
provider_slug: postmates
slug: postmates-domain-security
source_filename: postmates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: postmates.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 02:27:14 2026 GMT\n  hsts: null\n- host: developer.uber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\n- host: api.postmates.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 02:27:14 2026 GMT\n  hsts: null\ndomains:\n- domain: postmates.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: uber.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postmates/refs/heads/main/security/postmates-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Acquired
- Couriers
- Delivery
- Food Delivery
- Historical
- Logistics
- On-Demand
- Sunset
---
