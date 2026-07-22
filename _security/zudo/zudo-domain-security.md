---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: Quarantine
  dnssec: false
  domain: zudo.work
  spf: true
hosts:
- cert_expires: Sep 26 18:06:33 2026 GMT
  host: zudo.work
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zudo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zudo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=Quarantine).'
provider_name: Zudo
provider_slug: zudo
slug: zudo-domain-security
source_filename: zudo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zudo.work\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 18:06:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zudo.work\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: Quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zudo/refs/heads/main/security/zudo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Warranty
- Customer Service
- Customer Experience
- Automation
- Insurance
---
