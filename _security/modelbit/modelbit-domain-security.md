---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: modelbit.com
  spf: true
hosts:
- cert_expires: Oct 11 14:12:47 2026 GMT
  host: www.modelbit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modelbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modelbit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Modelbit
provider_slug: modelbit
slug: modelbit-domain-security
source_filename: modelbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.modelbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:12:47 2026 GMT\n  hsts: null\ndomains:\n- domain: modelbit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modelbit/refs/heads/main/security/modelbit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Machine Learning
- MLOps
- Model Deployment
- Model Inference
- Data Science
- Model Registry
---
