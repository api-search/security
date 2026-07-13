---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netflix.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netflixstudios.com
  spf: true
hosts:
- cert_expires: Feb 18 21:41:48 2027 GMT
  host: www.netflix.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 12:01:56 2026 GMT
  host: openconnect.netflix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 23:40:36 2026 GMT
  host: partnerhelp.netflixstudios.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netflix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netflix, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Netflix
provider_slug: netflix
slug: netflix-domain-security
source_filename: netflix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.netflix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 21:41:48 2027 GMT\n  hsts: null\n- host: openconnect.netflix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 12:01:56 2026 GMT\n  hsts: false\n- host: partnerhelp.netflixstudios.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:40:36 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: netflix.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: netflixstudios.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netflix/refs/heads/main/security/netflix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CDN
- Content Delivery
- Device Certification
- Entertainment
- Media
- Netflix
- Open Connect
- Streaming
- Fortune 500
---
