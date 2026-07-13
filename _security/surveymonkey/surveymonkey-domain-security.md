---
api_specs:
- filename: surveymonkey-openapi.yml
  format: yaml
  label: SurveyMonkey API v3
  slug: rest-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surveymonkey/refs/heads/main/openapi/surveymonkey-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: surveymonkey.com
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: api.surveymonkey.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Surveymonkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SurveyMonkey, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SurveyMonkey
provider_slug: surveymonkey
slug: surveymonkey-domain-security
source_filename: surveymonkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.surveymonkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: surveymonkey.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surveymonkey/refs/heads/main/security/surveymonkey-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Surveys
- Market Research
- Feedback
- NPS
- Forms
- OAuth
---
