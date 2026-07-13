---
api_specs:
- filename: microsoft-edge-addons-api.yaml
  format: yaml
  label: Microsoft Edge Add-ons API
  slug: edge-addons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/openapi/microsoft-edge-addons-api.yaml
- filename: microsoft-edge-devtools-api.yaml
  format: yaml
  label: Microsoft Edge DevTools Protocol HTTP API
  slug: edge-devtools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/openapi/microsoft-edge-devtools-api.yaml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 04:56:48 2026 GMT
  host: api.addons.microsoftedge.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 05:58:20 2026 GMT
  host: microsoftedge.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Edge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Edge, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Edge
provider_slug: microsoft-edge
slug: microsoft-edge-domain-security
source_filename: microsoft-edge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.addons.microsoftedge.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 04:56:48 2026 GMT\n  hsts: null\n- host: microsoftedge.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 05:58:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-edge/refs/heads/main/security/microsoft-edge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Browser
- Chromium
- Developer Tools
- Edge
- Extensions
- Microsoft
- Progressive Web Apps
- Web Development
- WebView
---
