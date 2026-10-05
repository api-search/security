---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: domino.ai
  spf: true
hosts:
- cert_expires: Nov 24 16:55:55 2026 GMT
  host: domino.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domino Data Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Domino Data Lab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Domino Data Lab
provider_slug: domino-data-lab
slug: domino-data-lab-domain-security
source_filename: domino-data-lab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domino.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 16:55:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: domino.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domino-data-lab/refs/heads/main/security/domino-data-lab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MLOps
- Data Science
- Machine Learning
- AI Platform
- Model Monitoring
- Enterprise AI
---
