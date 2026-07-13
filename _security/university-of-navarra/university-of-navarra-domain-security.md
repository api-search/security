---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unav.edu
  spf: true
hosts:
- cert_expires: Aug 14 12:02:55 2026 GMT
  host: en.unav.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 12:12:48 2026 GMT
  host: www.unav.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 04:30:04 2026 GMT
  host: dadun.unav.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Navarra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Navarra, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Navarra
provider_slug: university-of-navarra
slug: university-of-navarra-domain-security
source_filename: university-of-navarra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.unav.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 12:02:55 2026 GMT\n  hsts: false\n- host: www.unav.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 12:12:48 2026 GMT\n  hsts: false\n- host: dadun.unav.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 04:30:04 2026 GMT\n  hsts: null\ndomains:\n- domain: unav.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-navarra/refs/heads/main/security/university-of-navarra-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Spain
- Open Access
- Institutional Repository
- OAI-PMH
---
