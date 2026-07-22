---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lightanchor.ai
  spf: false
hosts:
- cert_expires: Sep 14 20:58:24 2026 GMT
  host: lightanchor.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Light Anchor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Light Anchor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Light Anchor
provider_slug: light-anchor
slug: light-anchor-domain-security
source_filename: light-anchor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightanchor.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:58:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lightanchor.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/light-anchor/refs/heads/main/security/light-anchor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- E-Commerce
- Consumer Brands
- AI Agents
- Automation
- Y Combinator
---
