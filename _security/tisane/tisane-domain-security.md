---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tisane.ai
  spf: true
hosts:
- cert_expires: Sep 14 11:17:34 2026 GMT
  host: tisane.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tisane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tisane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tisane
provider_slug: tisane
slug: tisane-domain-security
source_filename: tisane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tisane.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 14 11:17:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tisane.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tisane/refs/heads/main/security/tisane-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Text Analysis
- Public APIs
---
