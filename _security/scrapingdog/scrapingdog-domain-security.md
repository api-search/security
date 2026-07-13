---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: scrapingdog.com
  spf: true
hosts:
- cert_expires: Sep  1 12:49:04 2026 GMT
  host: www.scrapingdog.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scrapingdog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScrapingDog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ScrapingDog
provider_slug: scrapingdog
slug: scrapingdog-domain-security
source_filename: scrapingdog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scrapingdog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 12:49:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scrapingdog.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrapingdog/refs/heads/main/security/scrapingdog-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Development
- Public APIs
---
