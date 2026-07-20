---
api_specs:
- filename: azumio-food-recognition-openapi.yml
  format: yaml
  label: Calorie Mama Food Recognition API
  slug: calorie-mama-food-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azumio/refs/heads/main/openapi/azumio-food-recognition-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: azumio.com
  spf: true
hosts:
- cert_expires: Sep 14 11:02:03 2026 GMT
  host: azumio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Azumio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azumio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Azumio
provider_slug: azumio
slug: azumio-domain-security
source_filename: azumio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: azumio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 11:02:03 2026 GMT\n  hsts: false\ndomains:\n- domain: azumio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azumio/refs/heads/main/security/azumio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Health
- Digital Health
- Nutrition
- Food Recognition
- Machine Learning
- Artificial Intelligence
- Fitness
- Diabetes
- API
---
