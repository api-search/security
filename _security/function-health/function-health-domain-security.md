---
api_specs:
- filename: function-health-openapi.yml
  format: yaml
  label: Function Health Member Dashboard
  slug: function-health-member-dashboard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/function-health/refs/heads/main/openapi/function-health-openapi.yml
- filename: function-health-openapi.yml
  format: yaml
  label: Function Health Results Export
  slug: function-health-results-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/function-health/refs/heads/main/openapi/function-health-openapi.yml
- filename: function-health-openapi.yml
  format: yaml
  label: Function Health Connected Apps
  slug: function-health-connected-apps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/function-health/refs/heads/main/openapi/function-health-openapi.yml
- filename: function-health-openapi.yml
  format: yaml
  label: Function Health ChatGPT App
  slug: function-health-chatgpt-app
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/function-health/refs/heads/main/openapi/function-health-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: functionhealth.com
  spf: true
hosts:
- cert_expires: Sep 26 21:46:23 2026 GMT
  host: www.functionhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 10:05:19 2026 GMT
  host: my.functionhealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Function Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Function Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Function Health
provider_slug: function-health
slug: function-health-domain-security
source_filename: function-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.functionhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 21:46:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.functionhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 10:05:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: functionhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/function-health/refs/heads/main/security/function-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health
- Longevity
- Lab Testing
- Biomarkers
- Preventive Health
- Consumer Health
---
