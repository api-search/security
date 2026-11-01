---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trytrellis.co
  spf: false
hosts:
- cert_expires: Dec 23 04:54:35 2026 GMT
  host: www.trytrellis.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trytrellis Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trellis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Trellis
provider_slug: trytrellis-co
slug: trytrellis-co-domain-security
source_filename: trytrellis-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trytrellis.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 04:54:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trytrellis.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/trytrellis-co/security/trytrellis-co-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Low-code
- Integration
- Automation
- Enterprise
---
