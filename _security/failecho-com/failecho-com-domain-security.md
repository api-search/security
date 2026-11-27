---
api_specs:
- filename: failecho-com-network-api-openapi.yml
  format: yaml
  label: FailEcho Network API
  slug: failecho-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/failecho-com/openapi/failecho-com-network-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: failecho.com
  spf: true
hosts:
- cert_expires: Dec  9 12:38:46 2026 GMT
  host: failecho.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FailEcho Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FailEcho, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FailEcho
provider_slug: failecho-com
slug: failecho-com-domain-security
source_filename: failecho-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: failecho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 12:38:46 2026 GMT\n  hsts: null\ndomains:\n- domain: failecho.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/failecho-com/security/failecho-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Failure Intelligence
- Open Source
- Monitoring
- Free
- Platform
---
