---
api_specs:
- filename: develop-health-openapi.yml
  format: yaml
  label: Develop Health Public API
  slug: develop-health-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/develop-health/refs/heads/main/openapi/develop-health-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: develophealth.ai
  spf: true
hosts:
- cert_expires: Sep  2 13:35:46 2026 GMT
  host: www.develophealth.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 22:06:04 2026 GMT
  host: api.develophealth.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Develop Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Develop Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Develop Health
provider_slug: develop-health
slug: develop-health-domain-security
source_filename: develop-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.develophealth.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 13:35:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.develophealth.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:06:04 2026 GMT\n  hsts: null\ndomains:\n- domain: develophealth.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/develop-health/refs/heads/main/security/develop-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Prior Authorization
- Benefit Verification
- Medication Access
- Insurance
- Health Tech
- Artificial Intelligence
---
