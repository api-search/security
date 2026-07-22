---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: expectedparrot.com
  spf: true
hosts:
- cert_expires: Aug 22 02:33:56 2026 GMT
  host: www.expectedparrot.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Expected Parrot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Expected Parrot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Expected Parrot
provider_slug: expected-parrot
slug: expected-parrot-domain-security
source_filename: expected-parrot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.expectedparrot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:33:56 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: expectedparrot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expected-parrot/refs/heads/main/security/expected-parrot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Large Language Models
- Surveys
- Research
- Social Science
- Synthetic Data
- AI Agents
- Market Research
- Python
---
