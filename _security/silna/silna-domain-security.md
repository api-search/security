---
api_specs:
- filename: silna-openapi.json
  format: json
  label: Silna Public API
  slug: silna-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silna/refs/heads/main/openapi/silna-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: silnahealth.com
  spf: true
hosts:
- cert_expires: Aug 26 06:54:42 2026 GMT
  host: www.silnahealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: app.silnahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 00:35:12 2026 GMT
  host: docs.silnahealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Silna, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Silna
provider_slug: silna
slug: silna-domain-security
source_filename: silna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.silnahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:54:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.silnahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\n- host: docs.silnahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 00:35:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: silnahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silna/refs/heads/main/security/silna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automation
- Healthcare
- Prior Authorization
- Benefits Check
- Eligibility
- Insurance
- Revenue Cycle
- API
---
