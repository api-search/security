---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uniroma1.it
  spf: true
hosts:
- cert_expires: Nov  6 14:42:36 2026 GMT
  host: www.uniroma1.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 10:09:39 2026 GMT
  host: iris.uniroma1.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 12:24:48 2026 GMT
  host: sbs.uniroma1.it
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sapienza University Of Rome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sapienza University of Rome, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sapienza University of Rome
provider_slug: sapienza-university-of-rome
slug: sapienza-university-of-rome-domain-security
source_filename: sapienza-university-of-rome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uniroma1.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 14:42:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: iris.uniroma1.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 10:09:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sbs.uniroma1.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 12:24:48 2026 GMT\n  hsts: false\ndomains:\n- domain: uniroma1.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sapienza-university-of-rome/refs/heads/main/security/sapienza-university-of-rome-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Library
- OAI-PMH
- Italy
---
