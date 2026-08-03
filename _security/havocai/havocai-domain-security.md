---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: havocai.com
  spf: true
hosts:
- cert_expires: Sep 15 20:25:23 2026 GMT
  host: www.havocai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Havocai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HavocAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HavocAI
provider_slug: havocai
slug: havocai-domain-security
source_filename: havocai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.havocai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 20:25:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: havocai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/havocai/refs/heads/main/security/havocai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defense
- Defense Technology
- Autonomy
- Robotics
- Maritime
- Uncrewed Systems
- Artificial Intelligence
- Command and Control
- Aerospace and Defense
---
