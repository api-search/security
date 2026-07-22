---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getlighthouse.com
  spf: true
hosts:
- cert_expires: Oct  9 23:23:36 2026 GMT
  host: getlighthouse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Get Lighthouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Get Lighthouse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Get Lighthouse
provider_slug: get-lighthouse
slug: get-lighthouse-domain-security
source_filename: get-lighthouse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getlighthouse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:23:36 2026 GMT\n  hsts: false\ndomains:\n- domain: getlighthouse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/get-lighthouse/refs/heads/main/security/get-lighthouse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Management Training
- Leadership Development
- Coaching
- Online Courses
- One-on-Ones
- Team Management
- Education
---
