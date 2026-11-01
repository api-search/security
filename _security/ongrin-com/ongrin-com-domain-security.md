---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ongrin.com
  spf: true
hosts:
- cert_expires: Dec  1 06:54:11 2026 GMT
  host: ongrin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ongrin Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Grin
provider_slug: ongrin-com
slug: ongrin-com-domain-security
source_filename: ongrin-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ongrin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 06:54:11 2026 GMT\n  hsts: null\ndomains:\n- domain: ongrin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ongrin-com/security/ongrin-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
