---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: kyros.ai
  spf: true
hosts:
- cert_expires: Oct  1 08:20:46 2026 GMT
  host: kyros.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kyros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kyros College Prep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Kyros College Prep
provider_slug: kyros
slug: kyros-domain-security
source_filename: kyros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kyros.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:20:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kyros.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kyros/refs/heads/main/security/kyros-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Education
- EdTech
- College Admissions
- College Prep
- Artificial Intelligence
- Counseling
- Test Preparation
- Students
---
