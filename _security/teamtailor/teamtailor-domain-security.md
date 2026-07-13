---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: teamtailor.com
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.teamtailor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 02:40:02 2026 GMT
  host: docs.teamtailor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.teamtailor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teamtailor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teamtailor, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Teamtailor
provider_slug: teamtailor
slug: teamtailor-domain-security
source_filename: teamtailor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.teamtailor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.teamtailor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 02:40:02 2026 GMT\n  hsts: null\n- host: api.teamtailor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: teamtailor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamtailor/refs/heads/main/security/teamtailor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ATS
- Applicant Tracking
- Recruiting
- HR
- Hiring
- Employer Branding
---
