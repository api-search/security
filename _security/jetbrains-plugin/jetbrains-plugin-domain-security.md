---
api_specs:
- filename: jetbrains-plugin-openapi.yml
  format: yaml
  label: JetBrains Marketplace API
  slug: marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jetbrains-plugin/refs/heads/main/openapi/jetbrains-plugin-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jetbrains.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: plugins.jetbrains.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jetbrains Plugin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JetBrains Marketplace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JetBrains Marketplace
provider_slug: jetbrains-plugin
slug: jetbrains-plugin-domain-security
source_filename: jetbrains-plugin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plugins.jetbrains.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jetbrains.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetbrains-plugin/refs/heads/main/security/jetbrains-plugin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Plugins
- IDE
- Marketplace
- Developer Tools
- JetBrains
- IntelliJ
---
