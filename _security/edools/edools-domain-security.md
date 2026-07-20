---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: edools.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: myedools.com
  spf: false
hosts:
- cert_expires: Oct  3 00:58:43 2026 GMT
  host: edools.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:45:16 2026 GMT
  host: docs.edools.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 18:22:39 2026 GMT
  host: sua-escola.myedools.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edools, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Edools
provider_slug: edools
slug: edools-domain-security
source_filename: edools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:58:43 2026 GMT\n  hsts: false\n- host: docs.edools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:45:16 2026 GMT\n  hsts: false\n- host: sua-escola.myedools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 18:22:39 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: edools.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: myedools.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edools/refs/heads/main/security/edools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- E-Learning
- LMS
- Online Courses
- EdTech
- Content Management
- Digital Products
- Brazil
- REST
---
