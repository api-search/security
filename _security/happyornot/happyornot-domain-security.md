---
api_specs:
- filename: happyornot-openapi-original.yml
  format: yaml
  label: HappyOrNot Customer API v2
  slug: happyornot-customer-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/happyornot/refs/heads/main/openapi/happyornot-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: happy-or-not.com
  spf: true
hosts:
- cert_expires: Aug 30 04:03:07 2026 GMT
  host: happy-or-not.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: api.happy-or-not.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Happyornot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HappyOrNot, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HappyOrNot
provider_slug: happyornot
slug: happyornot-domain-security
source_filename: happyornot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: happy-or-not.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 04:03:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.happy-or-not.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: happy-or-not.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/happyornot/refs/heads/main/security/happyornot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Customer Experience
- Customer Feedback
- Surveys
- Analytics
- Voice of Customer
- Retail
- Feedback
---
