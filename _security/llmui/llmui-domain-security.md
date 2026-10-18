---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: llmui.org
  spf: true
hosts:
- cert_expires: Jan 14 15:19:18 2027 GMT
  host: llmui.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Llmui Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexios Technologies TF, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nexios Technologies TF
provider_slug: llmui
slug: llmui-domain-security
source_filename: llmui-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llmui.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 15:19:18 2027 GMT\n  hsts: false\ndomains:\n- domain: llmui.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llmui/refs/heads/main/security/llmui-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Orchestration
- Open-Source
- Enterprise
---
