---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: treatmyocd.com
  spf: true
hosts:
- cert_expires: Oct 21 14:23:05 2026 GMT
  host: www.treatmyocd.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 10:28:27 2026 GMT
  host: api.treatmyocd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: private application backend; root 302s to www.treatmyocd.com
  tls_version: TLSv1.3
- cert_expires: Sep  5 13:24:57 2026 GMT
  host: app.treatmyocd.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: authenticated member application
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nocd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NOCD, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NOCD
provider_slug: nocd
slug: nocd-domain-security
source_filename: nocd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.treatmyocd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 14:23:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.treatmyocd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 10:28:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: private application backend; root 302s to www.treatmyocd.com\n- host: app.treatmyocd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 13:24:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: authenticated member application\ndomains:\n- domain: treatmyocd.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n\
  \  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nocd/refs/heads/main/security/nocd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Mental Health
- Telehealth
- Digital Health
- Therapy
- Behavioral Health
- Consumer Application
---
