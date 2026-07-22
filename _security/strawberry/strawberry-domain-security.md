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
  domain: strawberrybrowser.com
  spf: true
hosts:
- cert_expires: Aug 17 19:57:40 2026 GMT
  host: strawberrybrowser.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Strawberry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strawberry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Strawberry
provider_slug: strawberry
slug: strawberry-domain-security
source_filename: strawberry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: strawberrybrowser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 19:57:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: strawberrybrowser.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/strawberry/refs/heads/main/security/strawberry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Agentic Browser
- AI Agents
- Browser
- Productivity
- Automation
- Web Scraping
---
