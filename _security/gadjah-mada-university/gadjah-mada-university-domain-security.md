---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ugm.ac.id
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: ugm.ac.id
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 27 19:09:10 2026 GMT
  host: repository.ugm.ac.id
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 30 19:07:19 2026 GMT
  host: dti.ugm.ac.id
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gadjah Mada University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gadjah Mada University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gadjah Mada University
provider_slug: gadjah-mada-university
slug: gadjah-mada-university-domain-security
source_filename: gadjah-mada-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ugm.ac.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: repository.ugm.ac.id\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 27 19:09:10 2026 GMT\n  hsts: null\n- host: dti.ugm.ac.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 19:07:19 2026 GMT\n  hsts: false\ndomains:\n- domain: ugm.ac.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/security/gadjah-mada-university-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Indonesia
- Research
- Open Data
- Library
- Repository
---
