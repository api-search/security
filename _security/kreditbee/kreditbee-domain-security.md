---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kreditbee.in
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: krazybee.com
  spf: true
hosts:
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: www.kreditbee.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: consumer website (single-page app)
  tls_version: TLSv1.3
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: kreditbee.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: apex (serves the same SPA)
  tls_version: TLSv1.3
- anonymous_response: 403 ForbiddenException (application/json)
  cert_expires: Apr 10 23:59:59 2027 GMT
  host: api.kreditbee.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: private mobile/web backend (AWS API Gateway behind Cloudflare)
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.krazybee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: KrazyBee Services Limited (RBI-registered NBFC) website
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kreditbee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KreditBee, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KreditBee
provider_slug: kreditbee
slug: kreditbee-domain-security
source_filename: kreditbee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + additional KreditBee hosts\nnote: >-\n  Every KreditBee host observed sits behind Cloudflare and terminates TLS 1.3 with HSTS\n  at the one-year maximum. Neither registrable domain is DNSSEC-signed. kreditbee.in\n  publishes a broad CAA policy naming six issuers; krazybee.com (the RBI-registered\n  NBFC arm, KrazyBee Services Limited) publishes no CAA record at all. Both domains\n  publish a hard-fail SPF record and a DMARC record at p=quarantine rather than\n  p=reject.\nhosts:\n- host: www.kreditbee.in\n  role: consumer website (single-page app)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kreditbee.in\n  role: apex (serves the same SPA)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kreditbee.in\n  role: private mobile/web\
  \ backend (AWS API Gateway behind Cloudflare)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  anonymous_response: 403 ForbiddenException (application/json)\n- host: www.krazybee.com\n  role: KrazyBee Services Limited (RBI-registered NBFC) website\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kreditbee.in\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n\
  - domain: krazybee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n  - {host: www.kreditbee.in, method: TLS handshake + HTTP HEAD}\n  - {host: kreditbee.in, method: TLS handshake + HTTP HEAD}\n  - {host: api.kreditbee.in, method: TLS handshake + HTTP HEAD, http_status: 403}\n  - {host: www.krazybee.com, method: TLS handshake + HTTP HEAD}\n  - {domain: kreditbee.in, method: 'dig DNSKEY/CAA/TXT/_dmarc'}\n  - {domain: krazybee.com, method: 'dig DNSKEY/CAA/TXT/_dmarc'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kreditbee/refs/heads/main/security/kreditbee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial-Services
- Fintech
- Lending
- Digital Lending
- Personal Loans
- Consumer Credit
- NBFC
- Credit Score
- India
- Mobile
---
