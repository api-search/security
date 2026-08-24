---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: togetherlabs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: imvu.com
  spf: true
hosts:
- cert_expires: Nov  4 13:06:26 2026 GMT
  host: togetherlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 12:05:02 2026 GMT
  host: api.imvu.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Imvu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Together Labs, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Together Labs
provider_slug: imvu
slug: imvu-domain-security
source_filename: imvu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: togetherlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 13:06:26 2026 GMT\n  hsts: false\n- host: api.imvu.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 20 12:05:02 2026 GMT\n  hsts: null\ndomains:\n- domain: togetherlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: imvu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imvu/refs/heads/main/security/imvu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Social Networking
- Virtual Worlds
- Metaverse
- Gaming
- Avatars
- Virtual Goods
- Marketplace
- User Generated Content
- Scripting
- Digital Currency
- Blockchain
---
