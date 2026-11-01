---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: traderwai.com
  spf: true
hosts:
- cert_expires: Dec  8 22:09:09 2026 GMT
  host: traderwai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Traderwai Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for traderwai-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: traderwai-com
provider_slug: traderwai-com
slug: traderwai-com-domain-security
source_filename: traderwai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: traderwai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 22:09:09 2026 GMT\n  hsts: false\ndomains:\n- domain: traderwai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/traderwai-com/security/traderwai-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Trading
- Brokerage
- Automation
- Platform
---
