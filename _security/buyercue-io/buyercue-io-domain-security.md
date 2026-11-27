---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: buyercue.io
  spf: false
hosts:
- cert_expires: Jan 10 17:35:18 2027 GMT
  host: buyercue.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BuyerCue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BuyerCue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BuyerCue
provider_slug: buyercue-io
slug: buyercue-io-domain-security
source_filename: buyercue-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buyercue.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 17:35:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buyercue.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/buyercue-io/security/buyercue-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- B2B
- Software-as-a-Service
- Leads
- Buying Signals
- Growth
---
