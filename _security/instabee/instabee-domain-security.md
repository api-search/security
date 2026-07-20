---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: instabee.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: budbee.com
  spf: true
hosts:
- cert_expires: Aug 24 10:11:01 2026 GMT
  host: instabee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 04:20:19 2026 GMT
  host: developer.budbee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 15:18:13 2026 GMT
  host: api.budbee.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instabee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instabee, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Instabee
provider_slug: instabee
slug: instabee-domain-security
source_filename: instabee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instabee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:11:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.budbee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:20:19 2026 GMT\n  hsts: false\n- host: api.budbee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:18:13 2026 GMT\n  hsts: null\ndomains:\n- domain: instabee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: budbee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instabee/refs/heads/main/security/instabee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Logistics
- Last-Mile Delivery
- Shipping
- E-commerce
- Parcel Lockers
- Returns
- Nordics
---
