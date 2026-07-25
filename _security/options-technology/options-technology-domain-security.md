---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: options-it.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: activfinancial.com
  spf: true
hosts:
- cert_expires: Oct 11 18:00:06 2026 GMT
  host: www.options-it.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 07:49:58 2026 GMT
  host: weboneapi.activfinancial.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: aop-ny4-replay.activfinancial.com
  https: false
kind: domain-security
layout: security
method: probed
name: Options Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Options Technology, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Options Technology
provider_slug: options-technology
slug: options-technology-domain-security
source_filename: options-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.options-it.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 18:00:06 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: weboneapi.activfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 07:49:58 2026 GMT\n  hsts: false\n- host: aop-ny4-replay.activfinancial.com\n  https: false\ndomains:\n- domain: options-it.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: activfinancial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/options-technology/refs/heads/main/security/options-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Market Data
- Real-Time
- Streaming
- Trading Infrastructure
- Exchange Data
- Managed Services
- Low Latency
---
