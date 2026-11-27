---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cobrain.space
  spf: true
hosts:
- cert_expires: Jan 29 21:05:40 2027 GMT
  host: cobrain.space
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cobrain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cobrain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cobrain
provider_slug: cobrain-space
slug: cobrain-space-domain-security
source_filename: cobrain-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cobrain.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 21:05:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cobrain.space\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cobrain-space/security/cobrain-space-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Memory
- MCP
- MCP Server
- Knowledge Management
- Markdown
- Note Taking
- Collaboration
- Artificial Intelligence
---
