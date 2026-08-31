---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sixfold.ai
  spf: true
hosts:
- cert_expires: Sep 12 16:46:49 2026 GMT
  host: www.sixfold.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sixfold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sixfold, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Sixfold
provider_slug: sixfold
slug: sixfold-domain-security
source_filename: sixfold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sixfold.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 16:46:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sixfold.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sixfold/refs/heads/main/security/sixfold-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- Underwriting
- Artificial Intelligence
- Insurtech
- Property And Casualty
- Life And Health
- Risk Assessment
- Submission Triage
- Document Processing
- Agentic AI
- Enterprise SaaS
---
