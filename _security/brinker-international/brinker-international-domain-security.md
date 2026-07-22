---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brinker.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chilis.com
  spf: true
hosts:
- cert_expires: Sep 14 00:49:02 2026 GMT
  host: www.brinker.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 23:59:42 2026 GMT
  host: www.chilis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 05:10:36 2026 GMT
  host: www.maggianos.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brinker International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brinker International, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brinker International
provider_slug: brinker-international
slug: brinker-international-domain-security
source_filename: brinker-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brinker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 00:49:02 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: www.chilis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 23:59:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.maggianos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:10:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: brinker.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: chilis.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brinker-international/refs/heads/main/security/brinker-international-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurants
- Casual Dining
- Food Service
- Franchise
- Chilis
- Maggianos
- Fortune 1000
---
