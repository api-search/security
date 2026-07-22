---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: iterative.health
  spf: true
hosts:
- cert_expires: Oct  4 12:59:07 2026 GMT
  host: iterative.health
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iterative Health Fka Iterative Scopes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iterative Health (fka Iterative Scopes), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Iterative Health (fka Iterative Scopes)
provider_slug: iterative-health-fka-iterative-scopes
slug: iterative-health-fka-iterative-scopes-domain-security
source_filename: iterative-health-fka-iterative-scopes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iterative.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:59:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iterative.health\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iterative-health-fka-iterative-scopes/refs/heads/main/security/iterative-health-fka-iterative-scopes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Clinical Research
- Life Sciences
- Artificial Intelligence
- Gastroenterology
- Biotechnology
- Clinical Trials
---
