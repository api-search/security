---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bopixel.com
  spf: false
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: bopixel.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bopixel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bopixel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bopixel
provider_slug: bopixel
slug: bopixel-domain-security
source_filename: bopixel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bopixel.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bopixel.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bopixel/refs/heads/main/security/bopixel-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Machine Vision
- Imaging
- Hardware
- China
---
