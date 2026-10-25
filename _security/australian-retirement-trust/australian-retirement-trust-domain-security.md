---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: art.com.au
  spf: true
hosts:
- cert_expires: Jan  7 09:49:50 2027 GMT
  host: art.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Australian Retirement Trust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australian Retirement Trust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Australian Retirement Trust
provider_slug: australian-retirement-trust
slug: australian-retirement-trust-domain-security
source_filename: australian-retirement-trust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: art.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 09:49:50 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: art.com.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-retirement-trust/refs/heads/main/security/australian-retirement-trust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Superannuation
- Retirement
- Financial Services
- Investments
- Australia
---
