---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: versatile.ai
  spf: true
hosts:
- cert_expires: Oct 11 08:34:58 2026 GMT
  host: www.versatile.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Versatileai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for versatile.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: versatile.ai
provider_slug: versatileai
slug: versatileai-domain-security
source_filename: versatileai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.versatile.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 08:34:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: versatile.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/versatileai/refs/heads/main/security/versatileai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Construction Technology
- Artificial Intelligence
- Crane Intelligence
- Jobsite Analytics
- IoT
- Hardware
---
