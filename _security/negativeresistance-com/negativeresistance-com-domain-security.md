---
api_specs:
- filename: negativeresistance-com-hope-api-openapi.yml
  format: yaml
  label: Negative Resistance Hope API
  slug: negativeresistance-com-hope-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/negativeresistance-com/openapi/negativeresistance-com-hope-api-openapi.yml
- filename: negativeresistance-com-mind-api-openapi.yml
  format: yaml
  label: Negative Resistance Mind API
  slug: negativeresistance-com-mind-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/negativeresistance-com/openapi/negativeresistance-com-mind-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: negativeresistance.com
  spf: false
hosts:
- cert_expires: Jan  2 15:23:26 2027 GMT
  host: negativeresistance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Negative Resistance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Negative Resistance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Negative Resistance
provider_slug: negativeresistance-com
slug: negativeresistance-com-domain-security
source_filename: negativeresistance-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: negativeresistance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 15:23:26 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: negativeresistance.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/negativeresistance-com/security/negativeresistance-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Intelligence
- Signals
- Funding
- Infrastructure
- Medical Research
---
