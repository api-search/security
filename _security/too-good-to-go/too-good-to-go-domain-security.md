---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:admin@toogoodtogo.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: toogoodtogo.com
  spf: true
hosts:
- cert_expires: Nov 15 09:24:37 2026 GMT
  host: www.toogoodtogo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Too Good To Go Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Too Good To Go, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Too Good To Go
provider_slug: too-good-to-go
slug: too-good-to-go-domain-security
source_filename: too-good-to-go-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.toogoodtogo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 09:24:37 2026 GMT\n  hsts: null\ndomains:\n- domain: toogoodtogo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:admin@toogoodtogo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/too-good-to-go/refs/heads/main/security/too-good-to-go-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food Waste
- Surplus Food
- Marketplace
- Sustainability
- Grocery Retail
- Consumer App
- Climate Tech
- B Corporation
- Denmark
---
