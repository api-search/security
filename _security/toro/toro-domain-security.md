---
api_specs:
- filename: toro-horizon360-openapi.yml
  format: yaml
  label: Toro Horizon360
  slug: horizon360
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-horizon360-openapi.yml
- filename: toro-intellidash-openapi.yml
  format: yaml
  label: Toro IntelliDash
  slug: intellidash
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-intellidash-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thetorocompany.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: toro.com
  spf: true
hosts:
- cert_expires: Sep 28 10:25:09 2026 GMT
  host: www.thetorocompany.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 16:46:31 2026 GMT
  host: horizon360.toro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: www.toro.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Toro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toro, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Toro
provider_slug: toro
slug: toro-domain-security
source_filename: toro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thetorocompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:25:09 2026 GMT\n  hsts: null\n- host: horizon360.toro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:46:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.toro.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: thetorocompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: toro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/security/toro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Landscaping
- Irrigation
- Golf
- Equipment
- Smart Connected Products
- Fleet Management
- Turf Management
- Fortune 1000
---
