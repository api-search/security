---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: entelo.com
  spf: true
hosts:
- cert_expires: Aug 29 11:34:54 2026 GMT
  host: www.entelo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Entelo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entelo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Entelo
provider_slug: entelo
slug: entelo-domain-security
source_filename: entelo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.entelo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 11:34:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: entelo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entelo/refs/heads/main/security/entelo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruiting
- Talent Acquisition
- Human Resources
- Sourcing
- Candidate Engagement
- Artificial Intelligence
- Applicant Tracking
---
