---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zapataquantum.com
  spf: true
hosts:
- cert_expires: Nov  1 04:51:17 2026 GMT
  host: zapataquantum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zapata Computing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zapata Quantum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zapata Quantum
provider_slug: zapata-computing
slug: zapata-computing-domain-security
source_filename: zapata-computing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zapataquantum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 04:51:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zapataquantum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zapata-computing/refs/heads/main/security/zapata-computing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Quantum Computing
- Quantum Software
- Artificial Intelligence
- Scientific Computing
- Workflow Orchestration
- Enterprise Software
- Open Source
- Research
---
