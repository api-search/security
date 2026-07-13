---
api_specs:
- filename: lightpanda-openapi.yml
  format: yaml
  label: Lightpanda CDP WebSocket Interface
  slug: lightpanda-cdp-websocket-interface
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightpanda/refs/heads/main/openapi/lightpanda-openapi.yml
- filename: lightpanda-asyncapi.yml
  format: yaml
  label: Lightpanda Cloud
  slug: lightpanda-cloud
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightpanda/refs/heads/main/asyncapi/lightpanda-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lightpanda.io
  spf: true
hosts:
- cert_expires: Aug 11 22:11:56 2026 GMT
  host: lightpanda.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
- cert_expires: Aug 12 02:27:05 2026 GMT
  host: cloud.lightpanda.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightpanda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightpanda, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lightpanda
provider_slug: lightpanda
slug: lightpanda-domain-security
source_filename: lightpanda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightpanda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 22:11:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: 127.0.0.1\n  https: false\n- host: cloud.lightpanda.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 02:27:05 2026 GMT\n  hsts: null\ndomains:\n- domain: lightpanda.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightpanda/refs/heads/main/security/lightpanda-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Headless Browser
- Browser Automation
- CDP
- WebSocket
- AI Agents
- Web Scraping
---
