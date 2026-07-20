---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: archive.com
  spf: true
hosts:
- cert_expires: Sep 28 15:09:05 2026 GMT
  host: api-docs.archive.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 18:05:39 2026 GMT
  host: app.archive.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Archive Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archive Technologies, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Archive Technologies
provider_slug: archive-technologies
slug: archive-technologies-domain-security
source_filename: archive-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api-docs.archive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 15:09:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.archive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 18:05:39 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: archive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archive-technologies/refs/heads/main/security/archive-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Creator Marketing
- Influencer Marketing
- Social Listening
- User Generated Content
- E-commerce
- GraphQL
- MCP
---
