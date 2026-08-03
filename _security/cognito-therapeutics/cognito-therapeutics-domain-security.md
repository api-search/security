---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cognitotx.com
  spf: true
hosts:
- cert_expires: Sep  9 10:57:30 2026 GMT
  host: www.cognitotx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cognito Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognito Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cognito Therapeutics
provider_slug: cognito-therapeutics
slug: cognito-therapeutics-domain-security
source_filename: cognito-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cognitotx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 10:57:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cognitotx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognito-therapeutics/refs/heads/main/security/cognito-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Care
- Medical Devices
- Neurotechnology
- Neuroscience
- Alzheimers Disease
- Clinical Trials
- Digital Therapeutics
- Biotechnology
---
