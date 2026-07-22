---
api_specs:
- filename: verdigris-technologies-data-v4-openapi.json
  format: json
  label: Verdigris Data API
  slug: verdigris-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/openapi/verdigris-technologies-data-v4-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verdigris.co
  spf: true
hosts:
- cert_expires: Sep  5 17:48:49 2026 GMT
  host: docs.verdigris.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 22:22:26 2026 GMT
  host: api.verdigris.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verdigris Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verdigris Technologies, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verdigris Technologies
provider_slug: verdigris-technologies
slug: verdigris-technologies-domain-security
source_filename: verdigris-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.verdigris.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 17:48:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.verdigris.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:22:26 2026 GMT\n  hsts: null\ndomains:\n- domain: verdigris.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verdigris-technologies/refs/heads/main/security/verdigris-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Energy Management
- Building Automation
- Smart Buildings
- IoT
- Sustainability
- Power Monitoring
- Time Series
- Analytics
- Electricity
---
