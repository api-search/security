---
api_specs:
- filename: layup-technologies-openapi-original.json
  format: json
  label: LayUp API
  slug: layup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/layup-technologies/refs/heads/main/openapi/layup-technologies-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: layup.co.za
  spf: true
hosts:
- cert_expires: Aug 30 08:10:59 2026 GMT
  host: layup.co.za
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 08:10:59 2026 GMT
  host: documentation.layup.co.za
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 08:10:59 2026 GMT
  host: api.layup.co.za
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Layup Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LayUp Technologies, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LayUp Technologies
provider_slug: layup-technologies
slug: layup-technologies-domain-security
source_filename: layup-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: layup.co.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:10:59 2026 GMT\n  hsts: false\n- host: documentation.layup.co.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:10:59 2026 GMT\n  hsts: false\n- host: api.layup.co.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:10:59 2026 GMT\n  hsts: null\ndomains:\n- domain: layup.co.za\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/layup-technologies/refs/heads/main/security/layup-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Lay-By
- Save Now Buy Later
- BNPL
- Instalments
- Fintech
- South Africa
- DebiCheck
- E-commerce
- Merchants
---
