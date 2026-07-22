---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sphinx.ai
  spf: true
hosts:
- cert_expires: Aug 24 04:29:12 2026 GMT
  host: sphinx.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sphinx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sphinx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sphinx
provider_slug: sphinx
slug: sphinx-domain-security
source_filename: sphinx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sphinx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 04:29:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sphinx.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sphinx/refs/heads/main/security/sphinx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Data Science
- Data Governance
- Analytics
- AI Agents
- Developer Tools
- Jupyter
- LLM
- Data Reliability
---
