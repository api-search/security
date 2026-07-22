---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sentisum.com
  spf: true
hosts:
- cert_expires: Oct 14 18:03:46 2026 GMT
  host: sentisum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asksenti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AskSenti, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AskSenti
provider_slug: asksenti
slug: asksenti-domain-security
source_filename: asksenti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sentisum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 18:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sentisum.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asksenti/refs/heads/main/security/asksenti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CX Intelligence
- Customer Experience
- Voice of Customer
- Sentiment Analysis
- Customer Support
- Analytics
- Artificial Intelligence
- SaaS
---
