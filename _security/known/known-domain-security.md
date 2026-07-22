---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: known.com
  spf: true
hosts:
- cert_expires: Sep 21 16:17:53 2026 GMT
  host: known.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Known Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Known, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Known
provider_slug: known
slug: known-domain-security
source_filename: known-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: known.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:17:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: known.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/known/refs/heads/main/security/known-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Dating
- Mobile
- Voice AI
- Artificial Intelligence
- Social
- iOS
---
