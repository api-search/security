---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apacorp.com
  spf: true
hosts:
- cert_expires: Sep 13 04:57:44 2026 GMT
  host: apacorp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APA Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: APA Corporation
provider_slug: apa
slug: apa-domain-security
source_filename: apa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apacorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:57:44 2026 GMT\n  hsts: false\ndomains:\n- domain: apacorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apa/refs/heads/main/security/apa-domain-security.yml
summary_line: TLSv1.3
tags:
- Oil And Gas
- Energy
- Exploration
- Production
---
