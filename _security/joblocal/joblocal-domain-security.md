---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joblocal.de
  spf: true
hosts:
- cert_expires: Oct 11 04:56:46 2026 GMT
  host: www.joblocal.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Joblocal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joblocal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Joblocal
provider_slug: joblocal
slug: joblocal-domain-security
source_filename: joblocal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joblocal.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 04:56:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: joblocal.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joblocal/refs/heads/main/security/joblocal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruiting
- Jobs
- HR Technology
- Job Portal
- Talent Acquisition
- Artificial Intelligence
- Labor Market
- Employment
- Germany
---
