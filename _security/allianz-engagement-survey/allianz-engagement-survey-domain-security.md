---
api_specs:
- filename: allianz-engagement-survey.yaml
  format: yaml
  label: Allianz Engagement Survey API
  slug: engagement-survey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/openapi/allianz-engagement-survey.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: allianz.com
  spf: true
hosts:
- cert_expires: Aug 12 16:58:20 2026 GMT
  host: www.allianz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  8 15:00:23 2026 GMT
  host: api.allianz.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allianz Engagement Survey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allianz Engagement Survey, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
slug: allianz-engagement-survey-domain-security
source_filename: allianz-engagement-survey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allianz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.allianz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 15:00:23 2026 GMT\n  hsts: null\ndomains:\n- domain: allianz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/security/allianz-engagement-survey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
---
