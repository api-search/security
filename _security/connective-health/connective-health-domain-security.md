---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: connectivehealth.io
  spf: true
hosts:
- cert_expires: Jan  5 07:49:14 2027 GMT
  host: connectivehealth.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Connective Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connective Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Connective Health
provider_slug: connective-health
slug: connective-health-domain-security
source_filename: connective-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connectivehealth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 07:49:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: connectivehealth.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connective-health/refs/heads/main/security/connective-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- AI
- Interoperability
- RiskAdjustment
---
