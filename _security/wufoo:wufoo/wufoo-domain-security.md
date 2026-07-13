---
api_specs:
- filename: wufoo-rest-v3-openapi.yml
  format: yaml
  label: Wufoo REST API v3
  slug: wufoo:rest-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo:wufoo/refs/heads/main/openapi/wufoo-rest-v3-openapi.yml
- filename: wufoo-webhooks-asyncapi.yml
  format: yaml
  label: Wufoo Webhooks
  slug: wufoo:webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo:wufoo/refs/heads/main/asyncapi/wufoo-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wufoo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: surveymonkey.com
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: www.wufoo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: help.surveymonkey.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wufoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wufoo, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wufoo
provider_slug: wufoo:wufoo
slug: wufoo-domain-security
source_filename: wufoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wufoo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.surveymonkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wufoo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: surveymonkey.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wufoo:wufoo/refs/heads/main/security/wufoo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Forms
- Form Builder
- Surveys
- Data Collection
- Webhooks
- Payments
- SurveyMonkey
---
