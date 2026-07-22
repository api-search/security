---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tuniu.com
  spf: true
hosts:
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: www.tuniu.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: developer.tuniu.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: api.tuniu.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tuniu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tuniu, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tuniu
provider_slug: tuniu
slug: tuniu-domain-security
source_filename: tuniu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tuniu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: false\n- host: developer.tuniu.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: false\n- host: api.tuniu.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tuniu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tuniu/refs/heads/main/security/tuniu-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Travel
- Tourism
- Online Travel Agency
- Open Platform
- China
- E-Commerce
---
