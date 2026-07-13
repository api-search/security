---
api_specs:
- filename: polytomic-openapi.json
  format: json
  label: Polytomic API
  slug: polytomic
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polytomic/refs/heads/main/openapi/polytomic-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: polytomic.com
  spf: true
hosts:
- cert_expires: Sep 19 18:12:59 2026 GMT
  host: www.polytomic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: app.polytomic.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Polytomic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polytomic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Polytomic
provider_slug: polytomic
slug: polytomic-domain-security
source_filename: polytomic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.polytomic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 18:12:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.polytomic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: polytomic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polytomic/refs/heads/main/security/polytomic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Integration
- Reverse ETL
- Unified API
- ELT
- Data Sync
---
