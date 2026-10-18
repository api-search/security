---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: castellum.ai
  spf: true
hosts:
- cert_expires: Dec 19 06:56:42 2026 GMT
  host: www.castellum.ai
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Castellum Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Castellum.AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Castellum.AI
provider_slug: castellum-ai
slug: castellum-ai-domain-security
source_filename: castellum-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.castellum.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 06:56:42 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: castellum.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/castellum-ai/refs/heads/main/security/castellum-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AML
- KYC
- Fintech
- Compliance
- Artificial Intelligence
---
