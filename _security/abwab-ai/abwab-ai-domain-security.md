---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: abwab.ai
  spf: true
hosts:
- cert_expires: Sep 19 17:31:09 2026 GMT
  host: abwab.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 14:03:57 2026 GMT
  host: api.abwab.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abwab Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abwab Ai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Abwab Ai
provider_slug: abwab-ai
slug: abwab-ai-domain-security
source_filename: abwab-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abwab.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 17:31:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.abwab.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 14:03:57 2026 GMT\n  hsts: false\ndomains:\n- domain: abwab.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abwab-ai/refs/heads/main/security/abwab-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MSME Lending
- Credit Intelligence
- Credit Decisioning
- Credit Scoring
- Fintech
- Embedded Finance
- Lending
- Saudi Arabia
- Artificial Intelligence
---
