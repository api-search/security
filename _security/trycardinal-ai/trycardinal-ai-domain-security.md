---
description: ''
domains:
- caa:
  - 0 iodef "mailto:jianna@trycardinal.ai"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trycardinal.ai
  spf: true
hosts:
- cert_expires: Sep 30 16:27:57 2026 GMT
  host: trycardinal.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trycardinal Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardinal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cardinal
provider_slug: trycardinal-ai
slug: trycardinal-ai-domain-security
source_filename: trycardinal-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trycardinal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:27:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: trycardinal.ai\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:jianna@trycardinal.ai\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trycardinal-ai/refs/heads/main/security/trycardinal-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Sales
- Outbound Sales
- Sales Automation
- Go-To-Market
- Machine Learning
---
