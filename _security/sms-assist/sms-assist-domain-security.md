---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lessen.com
  spf: true
hosts:
- cert_expires: Oct  3 16:44:19 2026 GMT
  host: www.lessen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:03:44 2026 GMT
  host: developers.lessen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:03:44 2026 GMT
  host: meshlive.lessen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sms Assist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMS Assist, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SMS Assist
provider_slug: sms-assist
slug: sms-assist-domain-security
source_filename: sms-assist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lessen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:44:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.lessen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:03:44 2026 GMT\n  hsts: false\n- host: meshlive.lessen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:03:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lessen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sms-assist/refs/heads/main/security/sms-assist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Facilities Management
- Property Maintenance
- Work Orders
- Field Service
- Maintenance
- Real Estate
- GraphQL
- Webhooks
- Vendor Network
---
