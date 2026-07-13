---
api_specs:
- filename: apiDocPro.html
  format: yaml
  label: Nexo Pro Trading API
  slug: nexo-pro-trading-api
  spec_type: OpenAPI
  url: https://pro.nexo.com/apiDocPro.html
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nexo.com
  spf: true
hosts:
- cert_expires: Sep 21 22:59:44 2026 GMT
  host: nexo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 03:19:06 2026 GMT
  host: pro.nexo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 03:19:06 2026 GMT
  host: pg.nexo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nexo
provider_slug: nexo
slug: nexo-domain-security
source_filename: nexo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 22:59:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pro.nexo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 03:19:06 2026 GMT\n  hsts: false\n- host: pg.nexo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 03:19:06 2026 GMT\n  hsts: false\ndomains:\n- domain: nexo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexo/refs/heads/main/security/nexo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Crypto
- Lending
- Earning
- Trading
- Payments
- Digital Assets
- DeFi
---
