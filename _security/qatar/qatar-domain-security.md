---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qu.edu.qa
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.qu.edu.qa
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 21 07:50:42 2026 GMT
  host: libguides.qu.edu.qa
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:07:17 2026 GMT
  host: qspace.qu.edu.qa
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qatar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qatar University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qatar University
provider_slug: qatar
slug: qatar-domain-security
source_filename: qatar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qu.edu.qa\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\n- host: libguides.qu.edu.qa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:50:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: qspace.qu.edu.qa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:07:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qu.edu.qa\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qatar/refs/heads/main/security/qatar-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Qatar
- Middle East
- Research
- Open Access
- Institutional Repository
- DSpace
- OAI-PMH
---
