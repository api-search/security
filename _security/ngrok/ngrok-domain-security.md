---
api_specs:
- filename: ngrok-api-openapi.yml
  format: yaml
  label: ngrok API
  slug: ngrok
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/openapi/ngrok-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ngrok.com
  spf: true
hosts:
- cert_expires: Sep 30 16:16:57 2026 GMT
  host: ngrok.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 18:07:14 2026 GMT
  host: api.ngrok.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ngrok Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ngrok, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ngrok
provider_slug: ngrok
slug: ngrok-domain-security
source_filename: ngrok-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ngrok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:16:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ngrok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 18:07:14 2026 GMT\n  hsts: null\ndomains:\n- domain: ngrok.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/security/ngrok-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Gateway
- API Gateway
- Compute
- Developer Tools
- Gateways
- Ingress
- Platform
- Proxies
- Servers
- Tunnels
---
