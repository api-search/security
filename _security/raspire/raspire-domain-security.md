---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: raspire.com
  spf: true
hosts:
- cert_expires: Sep 23 22:42:53 2026 GMT
  host: raspire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Raspire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Raspire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Raspire
provider_slug: raspire
slug: raspire-domain-security
source_filename: raspire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: raspire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:42:53 2026 GMT\n  hsts: false\ndomains:\n- domain: raspire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/raspire/refs/heads/main/security/raspire-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Security
- Mobile
- Application Security
- Runtime Application Self-Protection
- RASP
- Fraud Prevention
- API Security
---
