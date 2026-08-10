---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fractal.ai
  spf: true
hosts:
- cert_expires: Oct 17 13:29:11 2026 GMT
  host: fractal.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fractal Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fractal Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fractal Analytics
provider_slug: fractal-analytics
slug: fractal-analytics-domain-security
source_filename: fractal-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fractal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 13:29:11 2026 GMT\n  hsts: null\ndomains:\n- domain: fractal.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fractal-analytics/refs/heads/main/security/fractal-analytics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Analytics
- Data Engineering
- Consulting
- Agentic AI
- Enterprise AI
- Machine Learning
- Decision Intelligence
- Professional Services
---
