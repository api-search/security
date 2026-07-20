---
api_specs:
- filename: li-cor-intermediate-hobolink-openapi.json
  format: json
  label: HOBOLINK External API
  slug: hobolink-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/li-cor-intermediate/refs/heads/main/openapi/li-cor-intermediate-hobolink-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: licor.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: licor.cloud
  spf: true
hosts:
- cert_expires: Oct 13 04:13:29 2026 GMT
  host: www.licor.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 26 23:59:59 2026 GMT
  host: api.licor.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Li Cor Intermediate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LI-COR Intermediate, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LI-COR Intermediate
provider_slug: li-cor-intermediate
slug: li-cor-intermediate-domain-security
source_filename: li-cor-intermediate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.licor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 04:13:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.licor.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: licor.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: licor.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/li-cor-intermediate/refs/heads/main/security/li-cor-intermediate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Environmental Monitoring
- Greenhouse Gas
- Climate
- Agriculture
- Sensors
- Data Loggers
- IoT
- Scientific Instruments
- Life Sciences
- Time Series Data
---
