---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hanqigroup.com
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: en.hanqigroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: www.hanqigroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hanqigroup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hanqi Group, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hanqi Group
provider_slug: hanqigroup
slug: hanqigroup-domain-security
source_filename: hanqigroup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.hanqigroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.hanqigroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hanqigroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hanqigroup/refs/heads/main/security/hanqigroup-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Environmental Technology
- Wastewater Treatment
- Petrochemical
- Water Treatment
- China
---
