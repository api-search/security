---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fau.eu
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: fau.de
  spf: true
hosts:
- cert_expires: Nov 19 13:17:25 2026 GMT
  host: www.fau.eu
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 15:57:44 2026 GMT
  host: ub.fau.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 11:08:34 2026 GMT
  host: open.fau.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Friedrich Alexander Universitat Erlangen Nurnberg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Friedrich-Alexander-Universität Erlangen-Nürnberg, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Friedrich-Alexander-Universität Erlangen-Nürnberg
provider_slug: friedrich-alexander-universitat-erlangen-nurnberg
slug: friedrich-alexander-universitat-erlangen-nurnberg-domain-security
source_filename: friedrich-alexander-universitat-erlangen-nurnberg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fau.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 13:17:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: ub.fau.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 15:57:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open.fau.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 11:08:34 2026 GMT\n  hsts: false\ndomains:\n- domain: fau.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: fau.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/friedrich-alexander-universitat-erlangen-nurnberg/refs/heads/main/security/friedrich-alexander-universitat-erlangen-nurnberg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Repository
- Library
- Germany
---
