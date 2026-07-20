---
api_specs:
- filename: eden-health-grdn-openapi-original.json
  format: json
  label: Eden Health Grdn API
  slug: eden-health-grdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-health/refs/heads/main/openapi/eden-health-grdn-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: edenhealth.com
  spf: true
hosts:
- host: edenhealth.com
  https: false
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: api.edenhealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eden Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eden Health, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eden Health
provider_slug: eden-health
slug: eden-health-domain-security
source_filename: eden-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edenhealth.com\n  https: false\n- host: api.edenhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: edenhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eden-health/refs/heads/main/security/eden-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Primary Care
- Virtual Care
- Telehealth
- Digital Health
- Patient
- Appointments
---
