---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: autoscience.ai
  spf: true
hosts:
- cert_expires: Sep 30 12:41:14 2026 GMT
  host: www.autoscience.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autoscience Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autoscience, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Autoscience
provider_slug: autoscience
slug: autoscience-domain-security
source_filename: autoscience-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autoscience.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:41:14 2026 GMT\n  hsts: false\ndomains:\n- domain: autoscience.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autoscience/refs/heads/main/security/autoscience-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Ai
- Machine Learning
- AI Research
- Automated Research
- Model Training
- Frontier Models
---
