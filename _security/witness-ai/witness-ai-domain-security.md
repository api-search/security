---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: witness.ai
  spf: true
hosts:
- cert_expires: Feb 20 01:35:12 2027 GMT
  host: witness.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Witness Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Witness AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Witness AI
provider_slug: witness-ai
slug: witness-ai-domain-security
source_filename: witness-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: witness.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 01:35:12 2027 GMT\n  hsts: false\ndomains:\n- domain: witness.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/witness-ai/refs/heads/main/security/witness-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- AI Security
- AI Governance
- Security
- Compliance
- Observability
---
