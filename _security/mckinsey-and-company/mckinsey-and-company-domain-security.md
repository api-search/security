---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mckinsey.com
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: www.mckinsey.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mckinsey And Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for McKinsey & Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: McKinsey & Company
provider_slug: mckinsey-and-company
slug: mckinsey-and-company-domain-security
source_filename: mckinsey-and-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mckinsey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mckinsey.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mckinsey-and-company/refs/heads/main/security/mckinsey-and-company-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Consulting
- Management Consulting
- Strategy
- Professional Services
- MBB
- Big Three
- AI
- Data Science
- Digital Transformation
- Operations
- Research
- Insights
- Open Source
- Agentic AI
- Kubernetes
- Data Visualization
- Causal Inference
- QuantumBlack
- Lilli
- Industry Analysis
---
