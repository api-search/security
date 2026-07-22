---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tenzai.com
  spf: true
hosts:
- cert_expires: Aug 22 16:59:48 2026 GMT
  host: www.tenzai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tenzai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tenzai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tenzai
provider_slug: tenzai
slug: tenzai-domain-security
source_filename: tenzai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tenzai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 16:59:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tenzai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenzai/refs/heads/main/security/tenzai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Cybersecurity
- Security
- Artificial Intelligence
- Penetration Testing
- Application Security
- Agentic AI
- Offensive Security
---
