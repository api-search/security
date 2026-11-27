---
api_specs:
- filename: gimmetext-com-jobs-api-openapi.yml
  format: yaml
  label: GimmeText Jobs API
  slug: gimmetext-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gimmetext-com/openapi/gimmetext-com-jobs-api-openapi.yml
- filename: gimmetext-com-uploads-api-openapi.yml
  format: yaml
  label: GimmeText Uploads API
  slug: gimmetext-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gimmetext-com/openapi/gimmetext-com-uploads-api-openapi.yml
- filename: gimmetext-com-usage-api-openapi.yml
  format: yaml
  label: GimmeText Usage API
  slug: gimmetext-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gimmetext-com/openapi/gimmetext-com-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gimmetext.com
  spf: true
hosts:
- cert_expires: Jan  8 01:27:26 2027 GMT
  host: gimmetext.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GimmeText Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GimmeText, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GimmeText
provider_slug: gimmetext-com
slug: gimmetext-com-domain-security
source_filename: gimmetext-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gimmetext.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 01:27:26 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gimmetext.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gimmetext-com/security/gimmetext-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Transcription
- Audio
- Video
- Privacy
- Software-as-a-Service
---
