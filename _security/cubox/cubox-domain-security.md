---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cubox.pro
  spf: true
hosts:
- cert_expires: Nov  5 06:59:59 2026 GMT
  host: cubox.pro
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cubox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cubox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cubox
provider_slug: cubox
slug: cubox-domain-security
source_filename: cubox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cubox.pro\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  5 06:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cubox.pro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cubox/security/cubox-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- AI
- Reading
- Knowledge-Management
- Productivity
- Cross-Platform
---
