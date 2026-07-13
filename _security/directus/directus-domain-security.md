---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: directus.com
  spf: true
hosts:
- cert_expires: Aug 27 10:56:22 2026 GMT
  host: directus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Directus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Directus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Directus
provider_slug: directus
slug: directus-domain-security
source_filename: directus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: directus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 10:56:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: directus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/directus/refs/heads/main/security/directus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GraphQL
- REST API
- Headless CMS
- Data Platform
- Open Source
- SQL Database
- No-Code
- Content Management
- Real-Time
- MCP
---
