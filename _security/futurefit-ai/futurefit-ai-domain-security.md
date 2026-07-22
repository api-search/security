---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: futurefit.ai
  spf: true
hosts:
- cert_expires: Sep 13 09:00:41 2026 GMT
  host: futurefit.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Futurefit Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FutureFit AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FutureFit AI
provider_slug: futurefit-ai
slug: futurefit-ai-domain-security
source_filename: futurefit-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: futurefit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 09:00:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: futurefit.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/futurefit-ai/refs/heads/main/security/futurefit-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Workforce
- Artificial Intelligence
- Career Navigation
- Talent
- Human Resources
- Economic Development
- Enterprise
---
