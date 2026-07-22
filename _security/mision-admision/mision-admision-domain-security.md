---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: misionadmision.com
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: misionadmision.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mision Admision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mision Admision, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mision Admision
provider_slug: mision-admision
slug: mision-admision-domain-security
source_filename: mision-admision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: misionadmision.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: misionadmision.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mision-admision/refs/heads/main/security/mision-admision-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Education
- EdTech
- Exam Preparation
- Online Learning
- Mexico
- Consumer
---
