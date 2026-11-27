---
api_specs:
- filename: amazon-alexa-openapi-generated.yml
  format: yaml
  label: Amazon Alexa API
  slug: amazon-alexa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-alexa/openapi/_ae-authored/amazon-alexa-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: May 22 23:59:59 2027 GMT
  host: developer.amazon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amazon Alexa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Alexa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Alexa
provider_slug: amazon-alexa
slug: amazon-alexa-domain-security
source_filename: amazon-alexa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-alexa/security/amazon-alexa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Voice Assistant
- Cloud
- IoT
- Smart Home
- Developer Platform
---
