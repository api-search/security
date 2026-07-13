---
api_specs:
- filename: smartling-openapi.json
  format: json
  label: Smartling REST API
  slug: api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartling/refs/heads/main/openapi/smartling-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smartling.com
  spf: true
hosts:
- cert_expires: Oct  5 19:31:22 2026 GMT
  host: www.smartling.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 18:03:48 2026 GMT
  host: api-reference.smartling.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: api.smartling.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Smartling Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smartling, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Smartling
provider_slug: smartling
slug: smartling-domain-security
source_filename: smartling-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smartling.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:31:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-reference.smartling.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 18:03:48 2026 GMT\n  hsts: false\n- host: api.smartling.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: smartling.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartling/refs/heads/main/security/smartling-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Localization
- Translation
- TMS
- LinguisticAI
- Neural MT
- Enterprise
- REST
---
