---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getspiffy.com
  spf: true
hosts:
- cert_expires: Nov 13 07:25:56 2026 GMT
  host: www.getspiffy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 22:22:08 2026 GMT
  host: my.getspiffy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: fleet.getspiffy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: app.getspiffy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 14:02:01 2026 GMT
  host: blog.getspiffy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 01:03:48 2026 GMT
  host: status.getspiffy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Get Spiffy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spiffy, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spiffy
provider_slug: get-spiffy
slug: get-spiffy-domain-security
source_filename: get-spiffy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getspiffy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 07:25:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.getspiffy.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  cert_expires: Oct 15 22:22:08 2026 GMT\n  tls_version: TLSv1.3\n- host: fleet.getspiffy.com\n  https: true\n  hsts: false\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  tls_version: TLSv1.3\n- host: app.getspiffy.com\n  https: true\n  hsts: false\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  tls_version: TLSv1.3\n- host: blog.getspiffy.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  cert_expires: Nov 13 14:02:01 2026 GMT\n  tls_version: TLSv1.3\n- host: status.getspiffy.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  cert_expires: Oct 14 01:03:48 2026 GMT\n  tls_version: TLSv1.3\ndomains:\n- domain: getspiffy.com\n\
  \  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnote: Hosts beyond the apis.yml Website were discovered by DNS enumeration of getspiffy.com and probed\n  in the same pass.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/get-spiffy/refs/heads/main/security/get-spiffy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Mobile Vehicle Service
- Dealership Software
- Fleet Management
- Field Service Management
- Vehicle Inspection
- Scheduling and Dispatch
- B2B SaaS
---
