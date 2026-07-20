---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cogniac.ai
  spf: true
hosts:
- cert_expires: Sep 22 06:58:11 2026 GMT
  host: cogniac.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cogniac Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cogniac, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cogniac
provider_slug: cogniac
slug: cogniac-domain-security
source_filename: cogniac-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cogniac.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 06:58:11 2026 GMT\n  hsts: false\ndomains:\n- domain: cogniac.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cogniac/refs/heads/main/security/cogniac-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Computer Vision
- Artificial Intelligence
- Machine Learning
- Visual Inspection
- Defect Detection
- Edge AI
- Manufacturing
- Industrial IoT
- MLOps
---
