---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usefulapi.io
  spf: true
hosts:
- cert_expires: Dec 12 13:15:11 2026 GMT
  host: usefulapi.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Usefulapi Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for usefulapi-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: usefulapi-io
provider_slug: usefulapi-io
slug: usefulapi-io-domain-security
source_filename: usefulapi-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usefulapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 13:15:11 2026 GMT\n  hsts: false\ndomains:\n- domain: usefulapi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/usefulapi-io/security/usefulapi-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- MCP
- SaaS
- API Hosting
- Developer Tools
---
