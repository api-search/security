---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: causal.app
  spf: true
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: www.causal.app
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Causal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Causal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Causal
provider_slug: causal
slug: causal-domain-security
source_filename: causal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.causal.app\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: causal.app\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/causal/refs/heads/main/security/causal-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fintech
- Financial Planning
- FP&A
- Business Modeling
- Forecasting
- Spreadsheets
- xP&A
- SaaS
---
