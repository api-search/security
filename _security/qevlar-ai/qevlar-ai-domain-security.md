---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qevlar.com
  spf: true
hosts:
- cert_expires: Oct  2 06:16:15 2026 GMT
  host: www.qevlar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qevlar Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qevlar AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Qevlar AI
provider_slug: qevlar-ai
slug: qevlar-ai-domain-security
source_filename: qevlar-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qevlar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:16:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qevlar.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qevlar-ai/refs/heads/main/security/qevlar-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Engineering Services
- Security
- Cybersecurity
- Security Operations
- SOC
- Artificial Intelligence
- Threat Detection
- Incident Response
- SaaS
---
