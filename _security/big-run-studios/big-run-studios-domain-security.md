---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bigrunstudios.com
  spf: true
hosts:
- cert_expires: Dec 26 13:44:56 2026 GMT
  host: bigrunstudios.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Big Run Studios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Big Run Studios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Big Run Studios
provider_slug: big-run-studios
slug: big-run-studios-domain-security
source_filename: big-run-studios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bigrunstudios.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 13:44:56 2026 GMT\n  hsts: false\ndomains:\n- domain: bigrunstudios.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/big-run-studios/refs/heads/main/security/big-run-studios-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Gaming
- Mobile
- Casual
- Underserved
---
