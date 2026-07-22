---
api_specs:
- filename: pixlee-content-api-openapi.yml
  format: yaml
  label: Pixlee Content API
  slug: pixlee-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixlee/refs/heads/main/openapi/pixlee-content-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emplifi.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pixlee.com
  spf: true
hosts:
- cert_expires: Sep 27 09:15:52 2026 GMT
  host: emplifi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:43:26 2026 GMT
  host: developers.pixlee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: distillery.pixlee.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixlee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixlee, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pixlee
provider_slug: pixlee
slug: pixlee-domain-security
source_filename: pixlee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emplifi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:15:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.pixlee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:43:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: distillery.pixlee.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: emplifi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pixlee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixlee/refs/heads/main/security/pixlee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- User Generated Content
- Social Commerce
- Visual Marketing
- Content
- Media
- eCommerce
- Widgets
- Emplifi
---
