---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: komga.org
  spf: false
hosts:
- cert_expires: Dec 21 20:56:50 2026 GMT
  host: komga.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Komga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Komga, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Komga
provider_slug: komga
slug: komga-domain-security
source_filename: komga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: komga.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 20:56:50 2026 GMT\n  hsts: false\ndomains:\n- domain: komga.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/komga/security/komga-domain-security.yml
summary_line: TLSv1.3
tags:
- Media Server
- Comics
- Manga
- eBooks
- Open Source
- Community
---
