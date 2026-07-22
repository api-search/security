---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smartex.ai
  spf: true
hosts:
- cert_expires: Oct 11 12:42:40 2026 GMT
  host: www.smartex.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smartex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Smartex
provider_slug: smartex
slug: smartex-domain-security
source_filename: smartex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smartex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 12:42:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: smartex.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartex/refs/heads/main/security/smartex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Textiles
- Manufacturing
- Computer Vision
- Artificial Intelligence
- Quality Control
- Sustainability
- Industrial IoT
- Hardware
---
