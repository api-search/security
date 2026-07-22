---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: graphsafety.ai
  spf: true
hosts:
- cert_expires: Aug 30 15:11:31 2026 GMT
  host: graphsafety.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Graph Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graph AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Graph AI
provider_slug: graph-ai
slug: graph-ai-domain-security
source_filename: graph-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graphsafety.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:11:31 2026 GMT\n  hsts: false\ndomains:\n- domain: graphsafety.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graph-ai/refs/heads/main/security/graph-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Ml
- Pharmacovigilance
- Drug Safety
- Patient Safety
- Life Sciences
- Healthcare
- Regulatory Compliance
- SaaS
---
