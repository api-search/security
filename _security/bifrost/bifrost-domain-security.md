---
api_specs:
- filename: bifrost-http-gateway-api.yaml
  format: yaml
  label: Bifrost HTTP Gateway API
  slug: bifrost-http-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bifrost/refs/heads/main/openapi/bifrost-http-gateway-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getmaxim.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: getbifrost.ai
  spf: true
hosts:
- cert_expires: Sep  9 12:04:49 2026 GMT
  host: www.getmaxim.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 22:31:10 2026 GMT
  host: docs.getbifrost.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 14:57:48 2026 GMT
  host: pkg.go.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bifrost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bifrost, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bifrost
provider_slug: bifrost
slug: bifrost-domain-security
source_filename: bifrost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getmaxim.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 12:04:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.getbifrost.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 22:31:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: pkg.go.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:57:48 2026 GMT\n  hsts: false\ndomains:\n- domain: getmaxim.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getbifrost.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bifrost/refs/heads/main/security/bifrost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Gateway
- LLM
- Load Balancing
- Open Source
- OpenAI Compatible
- MCP
---
