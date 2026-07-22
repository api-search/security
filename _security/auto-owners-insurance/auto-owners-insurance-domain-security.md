---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: auto-owners.com
  spf: true
hosts:
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: www.auto-owners.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Auto Owners Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auto-Owners Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Auto-Owners Insurance
provider_slug: auto-owners-insurance
slug: auto-owners-insurance-domain-security
source_filename: auto-owners-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.auto-owners.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: auto-owners.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auto-owners-insurance/refs/heads/main/security/auto-owners-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Auto Insurance
- Home Insurance
- Life Insurance
- Business Insurance
- Mutual Insurance
- Independent Agents
---
