---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xund.ai
  spf: true
hosts:
- cert_expires: Jan  2 15:30:58 2027 GMT
  host: xund.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xund Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xund, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Xund
provider_slug: xund
slug: xund-domain-security
source_filename: xund-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xund.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 15:30:58 2027 GMT\n  hsts: false\ndomains:\n- domain: xund.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/xund/security/xund-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Health
- AI
- Healthcare
- Diagnostics
- Risk-Assessment
---
