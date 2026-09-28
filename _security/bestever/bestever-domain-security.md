---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bestever.ai
  spf: true
hosts:
- cert_expires: Oct 30 13:18:11 2026 GMT
  host: www.bestever.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bestever Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bestever, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bestever
provider_slug: bestever
slug: bestever-domain-security
source_filename: bestever-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bestever.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 13:18:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bestever.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bestever/refs/heads/main/security/bestever-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Advertising
- Marketing
- Creative
---
