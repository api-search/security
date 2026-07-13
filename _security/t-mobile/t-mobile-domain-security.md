---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:pki-admin@t-mobile.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: t-mobile.com
  spf: true
hosts:
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: www.t-mobile.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 11:13:19 2026 GMT
  host: developer.t-mobile.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: T Mobile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for T-Mobile, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: T-Mobile
provider_slug: t-mobile
slug: t-mobile-domain-security
source_filename: t-mobile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.t-mobile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.t-mobile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 11:13:19 2026 GMT\n  hsts: null\ndomains:\n- domain: t-mobile.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:pki-admin@t-mobile.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/t-mobile/refs/heads/main/security/t-mobile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Wireless
- Mobile
- 5G
---
