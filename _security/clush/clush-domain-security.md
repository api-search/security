---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clush.ai
  spf: true
hosts:
- cert_expires: Nov  9 06:03:36 2026 GMT
  host: www.clush.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clush Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clush, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clush
provider_slug: clush
slug: clush-domain-security
source_filename: clush-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clush.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 06:03:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: clush.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clush/refs/heads/main/security/clush-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Cloud
- Platform
- South Korea
---
