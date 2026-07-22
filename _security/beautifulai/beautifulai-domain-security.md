---
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@beautiful.ai"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beautiful.ai
  spf: true
hosts:
- cert_expires: Sep 13 14:57:23 2026 GMT
  host: www.beautiful.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beautifulai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for beautiful.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: beautiful.ai
provider_slug: beautifulai
slug: beautifulai-domain-security
source_filename: beautifulai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beautiful.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:57:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: beautiful.ai\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@beautiful.ai\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beautifulai/refs/heads/main/security/beautifulai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Presentations
- Slides
- Design
- Productivity
- Collaboration
- SaaS
---
