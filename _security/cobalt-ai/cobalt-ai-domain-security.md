---
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 128 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cobaltai.com
  spf: true
hosts:
- cert_expires: Sep  8 18:49:42 2026 GMT
  host: www.cobaltai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cobalt Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cobalt AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cobalt AI
provider_slug: cobalt-ai
slug: cobalt-ai-domain-security
source_filename: cobalt-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cobaltai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 18:49:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cobaltai.com\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 128 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cobalt-ai/refs/heads/main/security/cobalt-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Physical Security
- Security Automation
- Artificial Intelligence
- Video Monitoring
- Access Control
- Robotics
- Remote Monitoring
- Security Operations
---
