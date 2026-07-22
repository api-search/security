---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: axonlabs.co
  spf: true
hosts:
- cert_expires: Aug 21 05:55:39 2026 GMT
  host: www.axonlabs.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Axon
provider_slug: axon
slug: axon-domain-security
source_filename: axon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axonlabs.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 05:55:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axonlabs.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axon/refs/heads/main/security/axon-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Predictive Intelligence
- World Models
- Edge Computing
- Fintech
- High-Frequency Trading
- Robotics
---
