---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: refectory.fr
  spf: true
hosts:
- cert_expires: Sep 19 10:13:07 2026 GMT
  host: www.refectory.fr
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 10:14:25 2026 GMT
  host: customers.refectory.fr
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dejbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dejbox (Refectory), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dejbox (Refectory)
provider_slug: dejbox
slug: dejbox-domain-security
source_filename: dejbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.refectory.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 10:13:07 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: customers.refectory.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 10:14:25 2026 GMT\n  hsts: null\ndomains:\n- domain: refectory.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dejbox/refs/heads/main/security/dejbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food & Agritech
- Corporate Catering
- Food Delivery
- B2B
- France
- Meal Delivery
- OAuth2
- OpenID Connect
---
