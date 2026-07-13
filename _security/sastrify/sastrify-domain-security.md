---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@sastrify.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sastrify.com
  spf: true
hosts:
- cert_expires: Oct  5 11:29:02 2026 GMT
  host: www.sastrify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sastrify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sastrify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sastrify
provider_slug: sastrify
slug: sastrify-domain-security
source_filename: sastrify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sastrify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 11:29:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sastrify.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@sastrify.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sastrify/refs/heads/main/security/sastrify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cost Optimization
- License Management
- Procurement
- SaaS Management
- Software Spend
- Vendor Management
---
