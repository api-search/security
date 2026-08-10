---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ecr.ai
  spf: true
hosts:
- cert_expires: Sep 11 12:00:11 2026 GMT
  host: www.ecr.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edge Case Research Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edge Case Research, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Edge Case Research
provider_slug: edge-case-research
slug: edge-case-research-domain-security
source_filename: edge-case-research-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ecr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:00:11 2026 GMT\n  hsts: null\ndomains:\n- domain: ecr.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edge-case-research/refs/heads/main/security/edge-case-research-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Safety
- Functional Safety
- Autonomous Systems
- Robotics
- Artificial Intelligence
- Aerospace and Defense
- Automotive
- Risk Management
- Assurance
- Space
- Model Context Protocol
---
