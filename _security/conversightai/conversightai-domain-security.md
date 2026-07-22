---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: conversight.ai
  spf: true
hosts:
- cert_expires: Sep  1 19:16:32 2026 GMT
  host: conversight.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conversightai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConverSight.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ConverSight.ai
provider_slug: conversightai
slug: conversightai-domain-security
source_filename: conversightai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conversight.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 19:16:32 2026 GMT\n  hsts: false\ndomains:\n- domain: conversight.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conversightai/refs/heads/main/security/conversightai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Supply Chain
- Decision Intelligence
- Agentic AI
- Analytics
- Data
- Enterprise
- Manufacturing
---
