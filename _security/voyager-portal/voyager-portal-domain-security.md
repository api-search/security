---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: voyagerportal.com
  spf: true
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gitlab.com
  spf: true
hosts:
- cert_expires: Oct  3 15:46:14 2026 GMT
  host: voyagerportal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: gitlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: kong.voyagerportal.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Voyager Portal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voyager Portal, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Voyager Portal
provider_slug: voyager-portal
slug: voyager-portal-domain-security
source_filename: voyager-portal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voyagerportal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:46:14 2026 GMT\n  hsts: false\n- host: gitlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kong.voyagerportal.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: voyagerportal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n- domain: gitlab.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyager-portal/refs/heads/main/security/voyager-portal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Maritime
- Shipping
- Logistics
- Demurrage
- Laytime
- Voyages
- Workflows
- Bulk Commodities
---
