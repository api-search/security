---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: itrustcapital.com
  spf: true
hosts:
- cert_expires: Sep  6 00:59:44 2026 GMT
  host: www.itrustcapital.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 03:53:16 2026 GMT
  host: app.itrustcapital.com
  hsts: null
  https: true
  note: Application host (web app login/signup). Fronted by Cloudflare bot management — anonymous HEAD/GET returns HTTP 403 with a JS interstitial, so HSTS could not be observed. TLS handshake and certificate were observed directly.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Itrustcapital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iTrustCapital, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: iTrustCapital
provider_slug: itrustcapital
slug: itrustcapital-domain-security
source_filename: itrustcapital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.itrustcapital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 00:59:44 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: app.itrustcapital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 03:53:16 2026 GMT\n  hsts: null\n  note: 'Application host (web app login/signup). Fronted by Cloudflare bot management\n    — anonymous HEAD/GET returns HTTP 403 with a JS interstitial, so HSTS could not\n    be observed. TLS handshake and certificate were observed directly.'\ndomains:\n- domain: itrustcapital.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itrustcapital/refs/heads/main/security/itrustcapital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Cryptocurrency
- Digital Assets
- Retirement
- Individual Retirement Accounts
- Precious Metals
- Custody
- Fintech
- Wealth Management
- Staking
---
