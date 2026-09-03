---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vertoeducation.org
  spf: true
hosts:
- cert_expires: Nov  3 13:52:40 2026 GMT
  host: vertoeducation.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verto Education Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verto Education, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verto Education
provider_slug: verto-education
slug: verto-education-domain-security
source_filename: verto-education-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vertoeducation.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 13:52:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vertoeducation.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verto-education/refs/heads/main/security/verto-education-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Higher Education
- Study Abroad
- College Admissions
- Students
- Travel
- Model Context Protocol
- OAuth
- Agents
---
