---
api_specs:
- filename: rockwell-factorytalk-optix-openapi.yml
  format: yaml
  label: Rockwell FactoryTalk Optix REST API
  slug: factorytalk-optix-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockwell-factorytalk/refs/heads/main/openapi/rockwell-factorytalk-optix-openapi.yml
- filename: rockwell-factorytalk-realtime-asyncapi.yml
  format: yaml
  label: Rockwell FactoryTalk Hub API
  slug: factorytalk-hub-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockwell-factorytalk/refs/heads/main/asyncapi/rockwell-factorytalk-realtime-asyncapi.yml
description: ''
domains:
- caa:
  - 1 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: false
  domain: rockwellautomation.com
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: www.rockwellautomation.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: docs.rockwellautomation.com
  https: false
kind: domain-security
layout: security
method: probed
name: Rockwell Factorytalk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for rockwell-factorytalk, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: rockwell-factorytalk
provider_slug: rockwell-factorytalk
slug: rockwell-factorytalk-domain-security
source_filename: rockwell-factorytalk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rockwellautomation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.rockwellautomation.com\n  https: false\ndomains:\n- domain: rockwellautomation.com\n  dnssec: false\n  caa:\n  - 1 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockwell-factorytalk/refs/heads/main/security/rockwell-factorytalk-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags: []
---
