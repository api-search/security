---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rapidcanvas.ai
  spf: true
hosts:
- cert_expires: Sep 18 13:01:34 2026 GMT
  host: www.rapidcanvas.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 00:55:59 2026 GMT
  host: docs.rapidcanvas.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 04:53:57 2026 GMT
  host: app.rapidcanvas.ai
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rapidcanvas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RapidCanvas, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RapidCanvas
provider_slug: rapidcanvas
slug: rapidcanvas-domain-security
source_filename: rapidcanvas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rapidcanvas.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:01:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.rapidcanvas.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 00:55:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.rapidcanvas.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 04:53:57 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: rapidcanvas.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidcanvas/refs/heads/main/security/rapidcanvas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Agentic AI
- Data Science
- MLOps
- Enterprise AI
- AI Governance
- Low Code
- Developer Tools
---
