---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nexite.io
  spf: true
hosts:
- cert_expires: Sep 29 11:48:56 2026 GMT
  host: nexite.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nexite
provider_slug: nexite
slug: nexite-domain-security
source_filename: nexite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexite.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:48:56 2026 GMT\n  hsts: false\ndomains:\n- domain: nexite.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexite/refs/heads/main/security/nexite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- Retail Technology
- IoT
- Connected Retail
- Portfolio Company
---
