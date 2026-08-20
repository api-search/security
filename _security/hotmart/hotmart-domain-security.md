---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hotmart.com
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: hotmart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: developers.hotmart.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api-sec-vlc.hotmart.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hotmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hotmart, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hotmart
provider_slug: hotmart
slug: hotmart-domain-security
source_filename: hotmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hotmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.hotmart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: false\n- host: api-sec-vlc.hotmart.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hotmart.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotmart/refs/heads/main/security/hotmart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Creator Economy
- Digital Products
- Online Courses
- E-Commerce
- Payments
- Subscription
- Affiliate Marketing
- Webhook
- Learning Management
- Brazil
---
