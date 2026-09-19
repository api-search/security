---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: generallyintelligent.com
  spf: false
hosts:
- cert_expires: Nov  8 16:24:05 2026 GMT
  host: generallyintelligent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Generally Intelligent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Generally Intelligent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Generally Intelligent
provider_slug: generally-intelligent
slug: generally-intelligent-domain-security
source_filename: generally-intelligent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: generallyintelligent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 16:24:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: generallyintelligent.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nnote: generallyintelligent.com is the legacy brand domain of Imbue and now only 301s to imbue.com. It\n  still terminates TLS 1.3 with HSTS, but publishes no SPF, DMARC, CAA or DNSSEC — the retired domain\n  is spoofable as a sender. The live brand domain is probed on all/imbue.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/generally-intelligent/refs/heads/main/security/generally-intelligent-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Research
- Foundation Models
- Agents
- Reasoning
- Reinforcement Learning
- Open-Source
---
