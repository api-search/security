---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ucsf.edu
  spf: true
hosts:
- cert_expires: Aug  2 23:59:59 2026 GMT
  host: www.ucsf.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 13:20:57 2026 GMT
  host: profilesdeveloper.ucsf.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 04:51:25 2026 GMT
  host: api.profiles.ucsf.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ucsf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of California, San Francisco, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of California, San Francisco
provider_slug: ucsf
slug: ucsf-domain-security
source_filename: ucsf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucsf.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: profilesdeveloper.ucsf.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 13:20:57 2026 GMT\n  hsts: false\n- host: api.profiles.ucsf.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 04:51:25 2026 GMT\n  hsts: false\ndomains:\n- domain: ucsf.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucsf/refs/heads/main/security/ucsf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Health Sciences
- Research
- Researcher Profiles
- Open Data
- United States
---
