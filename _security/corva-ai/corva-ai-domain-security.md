---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: corva.ai
  spf: true
hosts:
- cert_expires: Sep 27 16:58:10 2026 GMT
  host: www.corva.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: api.corva.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: dc-docs.corva.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corva Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corva AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Corva AI
provider_slug: corva-ai
slug: corva-ai-domain-security
source_filename: corva-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.corva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:58:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.corva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dc-docs.corva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: corva.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corva-ai/refs/heads/main/security/corva-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Analytics
- Completions
- Custom Apps
- Data API
- Dev Center
- Drilling
- Energy
- Geoscience
- Oil and Gas
- Predictive Drilling
- Python SDK
- Real-time
- Sensor Data
- Sustainability
---
