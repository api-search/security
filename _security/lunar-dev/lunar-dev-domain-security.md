---
api_specs:
- filename: lunar-dev-gateway-admin-openapi.yml
  format: yaml
  label: Lunar.dev Gateway Admin API
  slug: gateway-admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-dev/refs/heads/main/openapi/lunar-dev-gateway-admin-openapi.yml
- filename: lunar-dev-gateway-proxy-openapi.yml
  format: yaml
  label: Lunar.dev Gateway Proxy API
  slug: gateway-proxy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lunar-dev/refs/heads/main/openapi/lunar-dev-gateway-proxy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lunar.dev
  spf: true
hosts:
- cert_expires: Sep  3 20:09:20 2026 GMT
  host: www.lunar.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 05:01:00 2026 GMT
  host: docs.lunar.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lunar Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lunar.dev, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lunar.dev
provider_slug: lunar-dev
slug: lunar-dev-domain-security
source_filename: lunar-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lunar.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 20:09:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lunar.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 05:01:00 2026 GMT\n  hsts: false\ndomains:\n- domain: lunar.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lunar-dev/refs/heads/main/security/lunar-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Gateway
- Automation
- Consumption Gateway
- Control
- Deployment
- Integrations
- MCP Gateway
- Performance
- Platform
- Version Control
- Visibility
- Workflows
---
