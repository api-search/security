---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ethon.ai
  spf: true
hosts:
- cert_expires: Oct  9 08:21:24 2026 GMT
  host: ethon.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ethonai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ethonai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ethonai
provider_slug: ethonai
slug: ethonai-domain-security
source_filename: ethonai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ethon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 08:21:24 2026 GMT\n  hsts: false\ndomains:\n- domain: ethon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ethonai/refs/heads/main/security/ethonai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Industrial AI
- Manufacturing
- Manufacturing Analytics
- Quality Management
- Machine Learning
- Causal AI
- Industry 4.0
- IoT
---
