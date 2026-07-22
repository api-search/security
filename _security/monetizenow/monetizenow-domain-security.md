---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: monetizenow.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: monetizeplatform.com
  spf: false
hosts:
- cert_expires: Sep 30 23:18:11 2026 GMT
  host: www.monetizenow.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 18:00:34 2026 GMT
  host: docs.monetizenow.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: api.monetizeplatform.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monetizenow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MonetizeNow, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MonetizeNow
provider_slug: monetizenow
slug: monetizenow-domain-security
source_filename: monetizenow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.monetizenow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:18:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.monetizenow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:00:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.monetizeplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: monetizenow.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: monetizeplatform.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monetizenow/refs/heads/main/security/monetizenow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Monetization
- Billing
- Subscriptions
- Usage-Based Pricing
- Quote-to-Cash
- CPQ
- Payments
- Invoicing
- Revenue
- SaaS
- FinTech
---
