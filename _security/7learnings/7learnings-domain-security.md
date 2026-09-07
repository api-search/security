---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: 7learnings.com
  spf: true
hosts:
- cert_expires: Nov 17 13:56:44 2026 GMT
  host: 7learnings.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 7Learnings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 7Learnings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: 7Learnings
provider_slug: 7learnings
slug: 7learnings-domain-security
source_filename: 7learnings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 7learnings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 13:56:44 2026 GMT\n  hsts: false\ndomains:\n- domain: 7learnings.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7learnings/refs/heads/main/security/7learnings-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Retail
- Pricing
- Price Optimization
- Predictive Pricing
- Demand Forecasting
- Machine Learning
- Ecommerce
- Performance Marketing
- Data Integration
- Germany
- SaaS
---
