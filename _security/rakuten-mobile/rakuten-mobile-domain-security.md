---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rakuten.co.jp
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rakuten.net
  spf: false
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: network.mobile.rakuten.co.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: corp.mobile.rakuten.co.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: portal.cpaas.symphony.rakuten.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rakuten Mobile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rakuten Mobile, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rakuten Mobile
provider_slug: rakuten-mobile
slug: rakuten-mobile-domain-security
source_filename: rakuten-mobile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: network.mobile.rakuten.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: corp.mobile.rakuten.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.cpaas.symphony.rakuten.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rakuten.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rakuten.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rakuten-mobile/refs/heads/main/security/rakuten-mobile-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Mobile Network Operator
- Carrier
- 5G
- 4G LTE
- Open RAN
- Cloud Native
- Symworld
- Symphony
- CPaaS
- SMS
- OTP
- Short URL
- Messaging
- OSS
- BSS
- RIC
- Kubernetes
- Edge
- Private 5G
- Japan
---
