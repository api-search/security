---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ub.edu
  spf: true
hosts:
- cert_expires: Nov 11 07:26:05 2026 GMT
  host: www.ub.edu
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 29 09:59:43 2026 GMT
  host: diposit.ub.edu
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: University Of Barcelona Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Barcelona, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Barcelona
provider_slug: university-of-barcelona
slug: university-of-barcelona-domain-security
source_filename: university-of-barcelona-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ub.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 07:26:05 2026 GMT\n  hsts: null\n- host: diposit.ub.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 09:59:43 2026 GMT\n  hsts: false\ndomains:\n- domain: ub.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-barcelona/refs/heads/main/security/university-of-barcelona-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Education
- Higher Education
- University
- Spain
- Catalonia
- Open Data
- Library
- Scholarly
- Repository
- DSpace
- OAI-PMH
---
