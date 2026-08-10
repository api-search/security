---
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sollishealth.com
  spf: true
hosts:
- cert_expires: Oct 13 07:46:34 2026 GMT
  host: www.sollishealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: mp.sollishealth.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: mp-api.sollishealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: navigator.sollishealth.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 10886400
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: navigator-api.sollishealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sollis Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sollis Health, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sollis Health
provider_slug: sollis-health
slug: sollis-health-domain-security
source_filename: sollis-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sollishealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 07:46:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mp.sollishealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: mp-api.sollishealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: null\n- host: navigator.sollishealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: navigator-api.sollishealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sollishealth.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0\
  \ issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sollis-health/refs/heads/main/security/sollis-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Healthcare
- Concierge Medicine
- Urgent Care
- Emergency Care
- Membership
- Telehealth
- HIPAA
---
