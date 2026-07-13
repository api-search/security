---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gotocompany.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gojek.com
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: www.gotocompany.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: www.gojek.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: api.gojekapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Goto Gojek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoTo Group (Gojek + Tokopedia), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GoTo Group (Gojek + Tokopedia)
provider_slug: goto-gojek
slug: goto-gojek-domain-security
source_filename: goto-gojek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gotocompany.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.gojek.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: null\n- host: api.gojekapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gotocompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gojek.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goto-gojek/refs/heads/main/security/goto-gojek-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Superapp
- Ride Hailing
- Food Delivery
- Last-Mile Logistics
- E-commerce
- Digital Payments
- Indonesia
- Southeast Asia
- Gojek
- Tokopedia
---
