---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openbazaar.org
  spf: false
hosts:
- cert_expires: Sep  1 11:35:26 2026 GMT
  host: openbazaar.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openbazaar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenBazaar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenBazaar
provider_slug: openbazaar
slug: openbazaar-domain-security
source_filename: openbazaar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openbazaar.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:35:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openbazaar.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openbazaar/refs/heads/main/security/openbazaar-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Marketplace
- Decentralized
- Peer-to-Peer
- Cryptocurrency
- Bitcoin
- E-Commerce
- Open Source
- Blockchain
---
