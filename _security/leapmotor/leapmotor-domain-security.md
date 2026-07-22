---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: leapmotor.net
  spf: false
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: false
  domain: leapmotor.cn
  spf: false
hosts:
- cert_expires: Aug 12 09:00:37 2026 GMT
  host: www.leapmotor.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: www.leapmotor.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Leapmotor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leapmotor, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Leapmotor
provider_slug: leapmotor
slug: leapmotor-domain-security
source_filename: leapmotor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leapmotor.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 09:00:37 2026 GMT\n  hsts: false\n- host: www.leapmotor.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: leapmotor.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: leapmotor.cn\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapmotor/refs/heads/main/security/leapmotor-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Technology
- Automotive
- Electric Vehicles
- Connected Vehicles
- Manufacturing
- Mobility
- China
---
