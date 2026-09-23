---
api_specs:
- filename: newminecraftservers-openapi.yml
  format: yaml
  label: NewMinecraftServers API
  slug: newminecraftservers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newminecraftservers/refs/heads/main/openapi/newminecraftservers-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: newminecraftservers.net
  spf: true
hosts:
- cert_expires: Dec 17 15:51:11 2026 GMT
  host: newminecraftservers.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Newminecraftservers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NewMinecraftServers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NewMinecraftServers
provider_slug: newminecraftservers
slug: newminecraftservers-domain-security
source_filename: newminecraftservers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: newminecraftservers.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 15:51:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: newminecraftservers.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newminecraftservers/refs/heads/main/security/newminecraftservers-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Minecraft
- Gaming
- server-directory
- Game Servers
- status-monitoring
- Public APIs
- Read Only
- JSON
---
