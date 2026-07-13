---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: resilinc.ai
  spf: true
hosts:
- cert_expires: Oct  8 08:57:45 2026 GMT
  host: resilinc.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Resilinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resilinc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Resilinc
provider_slug: resilinc
slug: resilinc-domain-security
source_filename: resilinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: resilinc.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:57:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: resilinc.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resilinc/refs/heads/main/security/resilinc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Supply Chain
- Risk Management
- Supplier Intelligence
- Disruption Monitoring
- AI
---
