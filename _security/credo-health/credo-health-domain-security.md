---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: credohealth.com
  spf: true
hosts:
- cert_expires: Jan  1 22:26:13 2027 GMT
  host: www.credohealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Credo Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credo Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Credo Health
provider_slug: credo-health
slug: credo-health-domain-security
source_filename: credo-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.credohealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 22:26:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: credohealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credo-health/refs/heads/main/security/credo-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- AI
- SaaS
- Value-Based Care
---
