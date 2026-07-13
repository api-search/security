---
api_specs:
- filename: bitrix24-openapi.json
  format: json
  label: Bitrix24 REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitrix24/refs/heads/main/openapi/bitrix24-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bitrix24.com
  spf: true
hosts:
- cert_expires: Dec 28 10:28:36 2026 GMT
  host: www.bitrix24.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 20:54:18 2026 GMT
  host: apidocs.bitrix24.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitrix24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitrix24, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bitrix24
provider_slug: bitrix24
slug: bitrix24-domain-security
source_filename: bitrix24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bitrix24.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 10:28:36 2026 GMT\n  hsts: false\n- host: apidocs.bitrix24.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 20:54:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bitrix24.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitrix24/refs/heads/main/security/bitrix24-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Collaboration
- Project Management
- Tasks
- Telephony
- Contact Center
- Document Management
- HR
- Business Suite
---
