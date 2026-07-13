---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: isct.ac.jp
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: titech.ac.jp
  spf: true
hosts:
- cert_expires: Oct 20 04:23:05 2026 GMT
  host: www.isct.ac.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 04:48:06 2027 GMT
  host: t2r2.star.titech.ac.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:48:07 2027 GMT
  host: www.gsic.titech.ac.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tokyo Institute Of Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tokyo Institute of Technology, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tokyo Institute of Technology
provider_slug: tokyo-institute-of-technology
slug: tokyo-institute-of-technology-domain-security
source_filename: tokyo-institute-of-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.isct.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 04:23:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: t2r2.star.titech.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 04:48:06 2027 GMT\n  hsts: false\n- host: www.gsic.titech.ac.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 23:48:07 2027 GMT\n  hsts: false\ndomains:\n- domain: isct.ac.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: titech.ac.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tokyo-institute-of-technology/refs/heads/main/security/tokyo-institute-of-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Japan
- Research
- Open Access
- Institutional Repository
- OAI-PMH
---
