---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cdbaby.com
  spf: true
hosts:
- cert_expires: Aug 19 05:01:26 2026 GMT
  host: cdbaby.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cd Baby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CD Baby, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CD Baby
provider_slug: cd-baby
slug: cd-baby-domain-security
source_filename: cd-baby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cdbaby.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 05:01:26 2026 GMT\n  hsts: false\ndomains:\n- domain: cdbaby.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cd-baby/refs/heads/main/security/cd-baby-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Music
- Music Distribution
- Music Publishing
- Publishing Administration
- Independent Artists
- Songwriters
- Streaming
- Sync Licensing
- Royalties
- Cover Song Licensing
- YouTube Monetization
- Performing Rights
- Physical Manufacturing
- Vinyl
- DIY Musician
---
