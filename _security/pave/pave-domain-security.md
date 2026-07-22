---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pave.com
  spf: true
hosts:
- cert_expires: Oct  3 16:02:38 2026 GMT
  host: www.pave.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pave
provider_slug: pave
slug: pave-domain-security
source_filename: pave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:02:38 2026 GMT\n  hsts: false\ndomains:\n- domain: pave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pave/refs/heads/main/security/pave-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Compensation
- Human Resources
- Compensation Benchmarking
- Market Data
- People Analytics
- HR Tech
- Total Rewards
---
