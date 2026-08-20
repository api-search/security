---
api_specs:
- filename: bfe-debug-api-openapi.yml
  format: yaml
  label: BFE Debug API
  slug: bfe-debug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/openapi/bfe-debug-api-openapi.yml
- filename: bfe-monitor-api-openapi.yml
  format: yaml
  label: BFE Monitor API
  slug: bfe-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/openapi/bfe-monitor-api-openapi.yml
- filename: bfe-reload-api-openapi.yml
  format: yaml
  label: BFE Reload API
  slug: bfe-reload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/openapi/bfe-reload-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bfe-networks.net
  spf: false
hosts:
- cert_expires: Sep 17 22:26:22 2026 GMT
  host: www.bfe-networks.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bfe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BFE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BFE
provider_slug: bfe
slug: bfe-domain-security
source_filename: bfe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bfe-networks.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:26:22 2026 GMT\n  hsts: false\ndomains:\n- domain: bfe-networks.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bfe/refs/heads/main/security/bfe-domain-security.yml
summary_line: TLSv1.3
tags:
- Load Balancer
- Networking
- Open-Source
- Traffic Management
- CNCF
- Baidu
---
