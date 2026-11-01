---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: elliat.nl
  spf: true
hosts:
- cert_expires: Dec 25 16:27:30 2026 GMT
  host: elliat.nl
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Elliat Nl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for elliat-nl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: elliat-nl
provider_slug: elliat-nl
slug: elliat-nl-domain-security
source_filename: elliat-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elliat.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 16:27:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: elliat.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/elliat-nl/security/elliat-nl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Developer
- JavaScript
- XML
- Fonto
- Consulting
---
