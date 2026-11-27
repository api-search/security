---
api_specs:
- filename: useproxy-dev-openapi-generated.yml
  format: yaml
  label: Proxy API
  slug: useproxy-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/useproxy-dev/openapi/_ae-authored/useproxy-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    agents: []
    checked: '2026-11-27'
    index:
    - alpn:
      - h2
      target: mcp.useproxy.dev
    published: true
  dnssec: true
  domain: useproxy.dev
  spf: true
hosts:
- cert_expires: Jan 18 18:01:51 2027 GMT
  host: useproxy.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Proxy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proxy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Proxy
provider_slug: useproxy-dev
slug: useproxy-dev-domain-security
source_filename: useproxy-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: useproxy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 18:01:51 2027 GMT\n  hsts: false\ndomains:\n- domain: useproxy.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-27'\n    published: true\n    index:\n    - target: mcp.useproxy.dev\n      alpn:\n      - h2\n    agents: []\n"
source_yaml_url: https://artifacts.apis.io/useproxy-dev/security/useproxy-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Advertising
- AI
- Marketing
- MCP
- Proxy
---
