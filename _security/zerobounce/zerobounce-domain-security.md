---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: zerobounce.net
  spf: true
hosts:
- cert_expires: Dec 19 19:59:26 2026 GMT
  host: www.zerobounce.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 19:59:26 2026 GMT
  host: api.zerobounce.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 19:59:26 2026 GMT
  host: api-eu.zerobounce.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zerobounce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZeroBounce, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ZeroBounce
provider_slug: zerobounce
slug: zerobounce-domain-security
source_filename: zerobounce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zerobounce.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 19:59:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.zerobounce.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 19:59:26 2026 GMT\n  hsts: null\n- host: api-eu.zerobounce.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 19:59:26 2026 GMT\n  hsts: null\ndomains:\n- domain: zerobounce.net\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerobounce/refs/heads/main/security/zerobounce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email Validation
- Email Deliverability
- Email Verification
- Marketing
- Lead Scoring
- Anti-Spam
---
