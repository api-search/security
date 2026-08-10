---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kueski.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kueskipay.com
  spf: true
hosts:
- cert_expires: Aug 23 23:59:59 2026 GMT
  host: www.kueski.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 08:21:05 2026 GMT
  host: www.kueskipay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: api.kueskipay.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kueski Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kueski, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kueski
provider_slug: kueski
slug: kueski-domain-security
source_filename: kueski-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kueski.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.kueskipay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 08:21:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kueskipay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: kueski.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kueskipay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kueski/refs/heads/main/security/kueski-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Buy Now Pay Later
- Lending
- Fintech
- Financial Services
- Consumer Credit
- E-Commerce
- Checkout
- Mexico
- Latin America
---
