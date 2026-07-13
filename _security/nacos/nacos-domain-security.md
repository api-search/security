---
api_specs:
- filename: nacos-open-api.yml
  format: yaml
  label: Nacos
  slug: nacos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/openapi/nacos-open-api.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nacos.io
  spf: false
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: nacos.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nacos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nacos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Nacos
provider_slug: nacos
slug: nacos-domain-security
source_filename: nacos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nacos.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nacos.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nacos/refs/heads/main/security/nacos-domain-security.yml
summary_line: TLSv1.3
tags:
- Alibaba
- Cloud Native
- Configuration Management
- DNS
- Java
- Microservices
- Service Discovery
- Service Management
---
