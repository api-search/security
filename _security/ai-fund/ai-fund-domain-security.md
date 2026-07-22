---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aifund.ai
  spf: true
hosts:
- cert_expires: Oct  6 04:22:56 2026 GMT
  host: aifund.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ai Fund Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Fund, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AI Fund
provider_slug: ai-fund
slug: ai-fund-domain-security
source_filename: ai-fund-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aifund.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:22:56 2026 GMT\n  hsts: false\ndomains:\n- domain: aifund.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-fund/refs/heads/main/security/ai-fund-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Venture Studio
- Venture Capital
- Artificial Intelligence
- Startups
- Investment
- Andrew Ng
---
