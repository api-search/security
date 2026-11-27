---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: curatorapproved.com
  spf: true
hosts:
- cert_expires: Jan  9 23:39:04 2027 GMT
  host: curatorapproved.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: The Curator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Curator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: The Curator
provider_slug: curatorapproved-com
slug: curatorapproved-com-domain-security
source_filename: curatorapproved-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curatorapproved.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:39:04 2027 GMT\n  hsts: false\ndomains:\n- domain: curatorapproved.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/curatorapproved-com/security/curatorapproved-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Curation
- Product Discovery
- Music
- Video
- Maker
- MCP
- Catalog
- RSS
---
