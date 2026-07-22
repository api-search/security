---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: herp.co.jp
  spf: true
hosts:
- cert_expires: Aug 21 09:55:16 2026 GMT
  host: herp.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Herp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HERP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HERP
provider_slug: herp
slug: herp-domain-security
source_filename: herp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: herp.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 09:55:16 2026 GMT\n  hsts: false\ndomains:\n- domain: herp.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/herp/refs/heads/main/security/herp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- HR Tech
- Recruiting
- Applicant Tracking
- ATS
- Human Resources
- SaaS
- Japan
---
