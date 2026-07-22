---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: seek.ai
  spf: true
hosts:
- cert_expires: Oct  1 03:01:29 2026 GMT
  host: www.seek.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seek Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seek AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Seek AI
provider_slug: seek-ai
slug: seek-ai-domain-security
source_filename: seek-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.seek.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:01:29 2026 GMT\n  hsts: null\ndomains:\n- domain: seek.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seek-ai/refs/heads/main/security/seek-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Generative AI
- Data Analytics
- Natural Language Query
- Enterprise Data
- Business Intelligence
- Acquired
- IBM watsonx
---
