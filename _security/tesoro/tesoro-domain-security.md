---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tesoro.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: archive.org
  spf: true
hosts:
- host: www.tesoro.com
  https: false
- cert_expires: Feb  9 22:02:42 2027 GMT
  host: web.archive.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 10:40:00 2026 GMT
  host: www.marathonpetroleum.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tesoro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tesoro, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tesoro
provider_slug: tesoro
slug: tesoro-domain-security
source_filename: tesoro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tesoro.com\n  https: false\n- host: web.archive.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 22:02:42 2027 GMT\n  hsts: false\n- host: www.marathonpetroleum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:40:00 2026 GMT\n  hsts: null\ndomains:\n- domain: tesoro.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: archive.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesoro/refs/heads/main/security/tesoro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Petroleum
- Refining
- Energy
- Oil And Gas
- Retail Fuel
- Fortune 100
---
