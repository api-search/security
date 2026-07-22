---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: si.inc
  spf: true
hosts:
- cert_expires: Sep 12 20:47:40 2026 GMT
  host: si.inc
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Standard Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Standard Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Standard Intelligence
provider_slug: standard-intelligence
slug: standard-intelligence-domain-security
source_filename: standard-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: si.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 20:47:40 2026 GMT\n  hsts: false\ndomains:\n- domain: si.inc\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/standard-intelligence/refs/heads/main/security/standard-intelligence-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Ai
- AGI
- Artificial Intelligence
- Machine Learning
- Foundation Models
- Speech AI
- Research
- Open Source
---
