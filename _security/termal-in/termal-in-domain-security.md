---
api_specs:
- filename: termal-in-openapi-generated.yml
  format: yaml
  label: Termalin API
  slug: termal-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/termal-in/openapi/_ae-authored/termal-in-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: termal.in
  spf: true
hosts:
- cert_expires: Feb 13 20:51:56 2027 GMT
  host: termal.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Termalin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Termalin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Termalin
provider_slug: termal-in
slug: termal-in-domain-security
source_filename: termal-in-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: termal.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 20:51:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: termal.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/termal-in/security/termal-in-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SSH
- MCP server
- Agent-native
- Remote desktop
- Server monitoring
- Backup
- Database client
- SFTP
---
