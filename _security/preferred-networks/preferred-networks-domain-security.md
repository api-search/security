---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: preferred.jp
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: preferredai.jp
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: www.preferred.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 13:21:39 2026 GMT
  host: docs.plamo.preferredai.jp
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 07:15:18 2026 GMT
  host: api.platform.preferredai.jp
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Preferred Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Preferred Networks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Preferred Networks
provider_slug: preferred-networks
slug: preferred-networks-domain-security
source_filename: preferred-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.preferred.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: false\n- host: docs.plamo.preferredai.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 13:21:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.platform.preferredai.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 07:15:18 2026 GMT\n  hsts: null\ndomains:\n- domain: preferred.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: preferredai.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preferred-networks/refs/heads/main/security/preferred-networks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Large Language Models
- Generative AI
- LLM Inference
- Foundation Models
- Japan
- Semiconductors
- Supercomputing
- Translation
- MCP
---
