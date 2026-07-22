---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hallo.ai
  spf: true
hosts:
- cert_expires: Aug 23 04:12:56 2026 GMT
  host: www.hallo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hallo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hallo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hallo
provider_slug: hallo
slug: hallo-domain-security
source_filename: hallo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hallo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 04:12:56 2026 GMT\n  hsts: false\ndomains:\n- domain: hallo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hallo/refs/heads/main/security/hallo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Language Assessment
- Language Learning
- Artificial Intelligence
- Recruiting
- Human Resources
- Education
- Speech Recognition
---
