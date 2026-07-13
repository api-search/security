---
api_specs:
- filename: chime-partner-api-openapi.yml
  format: yaml
  label: Chime Partner API
  slug: chime-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chime/refs/heads/main/openapi/chime-partner-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@chime.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chime.com
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "cloudflare.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chimebank.com
  spf: true
hosts:
- cert_expires: Sep 25 17:44:37 2026 GMT
  host: www.chime.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 20:19:25 2026 GMT
  host: developer.chime.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 20:44:34 2026 GMT
  host: api.chimebank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chime, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chime
provider_slug: chime
slug: chime-domain-security
source_filename: chime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:44:37 2026 GMT\n  hsts: null\n- host: developer.chime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 20:19:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.chimebank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:44:34 2026 GMT\n  hsts: null\ndomains:\n- domain: chime.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@chime.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: chimebank.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"cloudflare.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild\
  \ \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chime/refs/heads/main/security/chime-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Neobank
- Banking
- Checking Accounts
- Savings Accounts
- Early Paycheck Access
- Credit Building
- Peer-to-Peer Payments
- Consumer Banking
---
