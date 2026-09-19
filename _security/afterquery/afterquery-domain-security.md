---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: afterquery.com
  spf: true
hosts:
- cert_expires: Oct 21 16:24:12 2026 GMT
  host: www.afterquery.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 16:24:12 2026 GMT
  host: docs.afterquery.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Afterquery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AfterQuery, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AfterQuery
provider_slug: afterquery
slug: afterquery-domain-security
source_filename: afterquery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.afterquery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 16:24:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.afterquery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 16:24:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: afterquery.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afterquery/refs/heads/main/security/afterquery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- Training Data
- Data
- Evaluation
- Reinforcement Learning
- Benchmarks
- Research
- Agents
- MCP
---
