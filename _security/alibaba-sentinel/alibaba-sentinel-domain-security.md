---
api_specs:
- filename: sentinel-dashboard-api.yml
  format: yaml
  label: Sentinel Dashboard API
  slug: sentinel-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alibaba-sentinel/refs/heads/main/openapi/sentinel-dashboard-api.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sentinelguard.io
  spf: false
hosts:
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: sentinelguard.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Alibaba Sentinel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alibaba Sentinel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Alibaba Sentinel
provider_slug: alibaba-sentinel
slug: alibaba-sentinel-domain-security
source_filename: alibaba-sentinel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sentinelguard.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sentinelguard.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alibaba-sentinel/refs/heads/main/security/alibaba-sentinel-domain-security.yml
summary_line: TLSv1.2
tags:
- Alibaba
- Circuit Breaker
- Flow Control
- Java
- Microservices
- Rate Limiting
- Resilience
- Traffic Shaping
- Open Source
- Cloud Native
- Spring Cloud
---
