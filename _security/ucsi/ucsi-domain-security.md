---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ucsiuniversity.edu.my
  spf: true
hosts:
- cert_expires: Oct  6 00:27:52 2026 GMT
  host: www.ucsiuniversity.edu.my
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 00:27:52 2026 GMT
  host: koha.ucsiuniversity.edu.my
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ucsi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UCSI University, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: UCSI University
provider_slug: ucsi
slug: ucsi-domain-security
source_filename: ucsi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucsiuniversity.edu.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:27:52 2026 GMT\n  hsts: false\n- host: koha.ucsiuniversity.edu.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:27:52 2026 GMT\n  hsts: null\ndomains:\n- domain: ucsiuniversity.edu.my\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucsi/refs/heads/main/security/ucsi-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Malaysia
- Library
- Koha
---
