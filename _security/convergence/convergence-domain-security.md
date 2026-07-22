---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: convergence.ai
  spf: true
hosts:
- cert_expires: Sep 21 12:42:01 2026 GMT
  host: convergence.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Convergence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for convergence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: convergence
provider_slug: convergence
slug: convergence-domain-security
source_filename: convergence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: convergence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 12:42:01 2026 GMT\n  hsts: null\ndomains:\n- domain: convergence.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convergence/refs/heads/main/security/convergence-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Machine Learning
- Web Automation
- Open Weights
- Developer Tools
---
