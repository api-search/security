---
api_specs:
- filename: have-i-been-pwned-openapi.json
  format: json
  label: Have I Been Pwned API v3
  slug: api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/openapi/have-i-been-pwned-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: haveibeenpwned.com
  spf: true
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: pwnedpasswords.com
  spf: false
hosts:
- cert_expires: Oct  4 17:44:25 2026 GMT
  host: haveibeenpwned.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 01:27:37 2026 GMT
  host: api.pwnedpasswords.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Have I Been Pwned Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Have I Been Pwned, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Have I Been Pwned
provider_slug: have-i-been-pwned
slug: have-i-been-pwned-domain-security
source_filename: have-i-been-pwned-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: haveibeenpwned.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 17:44:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pwnedpasswords.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 01:27:37 2026 GMT\n  hsts: null\ndomains:\n- domain: haveibeenpwned.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pwnedpasswords.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n\
  \  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/have-i-been-pwned/refs/heads/main/security/have-i-been-pwned-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Data Breaches
- Pwned Passwords
- Identity
- Threat Intelligence
- Credential Stuffing
---
