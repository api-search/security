---
api_specs:
- filename: docontrol-openapi.yml
  format: yaml
  label: DoControl
  slug: docontrol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docontrol/refs/heads/main/openapi/docontrol-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: docontrol.io
  spf: true
hosts:
- cert_expires: Sep 30 08:31:32 2026 GMT
  host: www.docontrol.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: apollo-gateway-v4-api.prod.docontrol.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: auth.prod.docontrol.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Docontrol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DoControl, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DoControl
provider_slug: docontrol
slug: docontrol-domain-security
source_filename: docontrol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docontrol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 08:31:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apollo-gateway-v4-api.prod.docontrol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: null\n- host: auth.prod.docontrol.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: docontrol.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docontrol/refs/heads/main/security/docontrol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Security
- SaaS Security
---
