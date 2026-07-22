---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tucows.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opensrs.guide
  spf: false
hosts:
- cert_expires: Sep 11 16:28:54 2026 GMT
  host: tucows.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 20:40:57 2026 GMT
  host: domains.opensrs.guide
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: rr-n1-tor.opensrs.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tucows Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tucows, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tucows
provider_slug: tucows
slug: tucows-domain-security
source_filename: tucows-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tucows.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 16:28:54 2026 GMT\n  hsts: false\n- host: domains.opensrs.guide\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:40:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rr-n1-tor.opensrs.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tucows.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: opensrs.guide\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tucows/refs/heads/main/security/tucows-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure
- Domains
- DNS
- SSL
- Email
- Registrar
- Telecom
---
