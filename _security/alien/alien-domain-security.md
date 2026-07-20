---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alien.org
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: alien-api.com
  spf: false
hosts:
- cert_expires: Oct 10 01:55:49 2026 GMT
  host: alien.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 23:26:33 2026 GMT
  host: docs.alien.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 14:37:56 2026 GMT
  host: sso.alien-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alien Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alien, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Alien
provider_slug: alien
slug: alien-domain-security
source_filename: alien-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alien.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 01:55:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.alien.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 23:26:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sso.alien-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 14:37:56 2026 GMT\n  hsts: null\ndomains:\n- domain: alien.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: alien-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alien/refs/heads/main/security/alien-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Identity
- Authentication
- OAuth
- OpenID Connect
- Proof of Humanity
- Blockchain
- Solana
- Agents
---
