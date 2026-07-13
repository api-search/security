---
api_specs:
- filename: openapi.json
  format: json
  label: Temenos Transact Core Banking API
  slug: temenos-transact-core-banking-api
  spec_type: OpenAPI
  url: https://developer.temenos.com/transact/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: temenos.com
  spf: true
hosts:
- cert_expires: Sep 30 20:13:58 2026 GMT
  host: developer.temenos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 30 20:13:58 2026 GMT
  host: www.temenos.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 14 23:59:59 2026 GMT
  host: api.temenos.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Temenos Transact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Temenos Transact, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Temenos Transact
provider_slug: temenos-transact
slug: temenos-transact-domain-security
source_filename: temenos-transact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.temenos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 20:13:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.temenos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 20:13:58 2026 GMT\n  hsts: false\n- host: api.temenos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: temenos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/security/temenos-transact-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
---
