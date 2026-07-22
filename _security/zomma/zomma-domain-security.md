---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zommalabs.com
  spf: true
hosts:
- cert_expires: Oct 10 22:03:40 2026 GMT
  host: zommalabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zomma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zomma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zomma
provider_slug: zomma
slug: zomma-domain-security
source_filename: zomma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zommalabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 22:03:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zommalabs.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zomma/refs/heads/main/security/zomma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Computer Use
- Automation
- Fintech
- Back Office
- Reconciliation
- KYC
- Finance
---
