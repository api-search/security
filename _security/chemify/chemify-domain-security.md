---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chemify.io
  spf: true
hosts:
- cert_expires: Oct 11 09:08:52 2026 GMT
  host: www.chemify.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chemify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chemify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chemify
provider_slug: chemify
slug: chemify-domain-security
source_filename: chemify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chemify.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 09:08:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chemify.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chemify/refs/heads/main/security/chemify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Chemistry
- Programmable Chemistry
- Robotics
- Artificial Intelligence
- Machine Learning
- Drug Discovery
- Materials Science
- Automation
- Molecular Design
---
