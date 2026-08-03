---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bitfury.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: exonum.com
  spf: true
hosts:
- cert_expires: Sep 19 02:58:55 2026 GMT
  host: bitfury.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 21:54:27 2026 GMT
  host: exonum.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitfury Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BitFury, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BitFury
provider_slug: bitfury-group
slug: bitfury-group-domain-security
source_filename: bitfury-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitfury.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 02:58:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: exonum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 21:54:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bitfury.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: exonum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitfury-group/refs/heads/main/security/bitfury-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Bitcoin
- Cryptocurrency
- Distributed Ledger
- Permissioned Blockchain
- Open Source
- Data Centers
- Mining Hardware
- Enterprise Blockchain
---
