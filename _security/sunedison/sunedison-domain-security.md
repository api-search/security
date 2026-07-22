---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sunedison.com
  spf: true
hosts:
- cert_expires: Nov 28 05:05:42 2026 GMT
  host: www.sunedison.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sunedison Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SunEdison, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SunEdison
provider_slug: sunedison
slug: sunedison-domain-security
source_filename: sunedison-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sunedison.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 05:05:42 2026 GMT\n  hsts: false\ndomains:\n- domain: sunedison.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunedison/refs/heads/main/security/sunedison-domain-security.yml
summary_line: TLSv1.3
tags:
- Solar Energy
- Renewable Energy
- Wind Energy
- Clean Energy
- Energy
- Fortune 1000
---
