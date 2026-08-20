---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scalarr.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: edgelabs.ai
  spf: true
hosts:
- cert_expires: Nov  8 17:53:41 2026 GMT
  host: scalarr.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: edgelabs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: portal.edgelabs.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scalarr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scalarr, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scalarr
provider_slug: scalarr
slug: scalarr-domain-security
source_filename: scalarr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scalarr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 17:53:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: edgelabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.edgelabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: scalarr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: edgelabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalarr/refs/heads/main/security/scalarr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Runtime Security
- AI Agent Security
- Container Security
- Kubernetes
- Edge Computing
- Vulnerability Management
- Compliance
- NIS2
- Machine-Learning
- Artificial Intelligence
- Open-Source
- Fraud Detection
- Mobile Ad Fraud
---
