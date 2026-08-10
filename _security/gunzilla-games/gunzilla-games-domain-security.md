---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gunzillagames.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gunbygunz.com
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: gunzscan.io
  spf: false
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: gunztoken.io
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: gunzchain.io
  spf: false
hosts:
- cert_expires: Oct 24 13:59:55 2026 GMT
  host: gunzillagames.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 00:37:22 2026 GMT
  host: gunbygunz.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 04:29:41 2026 GMT
  host: rpc.gunzchain.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 02:47:27 2026 GMT
  host: gunzscan.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 21:41:05 2026 GMT
  host: api.gunztoken.io
  hsts: null
  https: true
  note: HTTP 403 - Cloudflare bot challenge on all paths except /.well-known/*
  tls_version: TLSv1.3
- cert_expires: Oct 28 05:00:06 2026 GMT
  host: marketplace.gunztoken.io
  hsts: null
  https: true
  note: HTTP 403 - Cloudflare bot challenge
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gunzilla Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gunzilla Games, probed live across 6 host(s) and 5 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gunzilla Games
provider_slug: gunzilla-games
slug: gunzilla-games-domain-security
source_filename: gunzilla-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + GUNZ chain/explorer/marketplace hosts\nhosts:\n- host: gunzillagames.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 13:59:55 2026 GMT\n  hsts: null\n- host: gunbygunz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 00:37:22 2026 GMT\n  hsts: null\n- host: rpc.gunzchain.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 04:29:41 2026 GMT\n  hsts: null\n- host: gunzscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 02:47:27 2026 GMT\n  hsts: null\n- host: api.gunztoken.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 21:41:05 2026 GMT\n  hsts: null\n  note: HTTP 403 - Cloudflare bot challenge on all paths except /.well-known/*\n- host: marketplace.gunztoken.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 05:00:06 2026 GMT\n  hsts: null\n  note: HTTP 403 - Cloudflare bot challenge\n\
  domains:\n- domain: gunzillagames.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gunbygunz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: gunzscan.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n- domain: gunztoken.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dmarc_policy: null\n- domain: gunzchain.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\nnotes: No host advertises HSTS. No domain publishes CAA or DNSSEC. gunzillagames.com publishes SPF + DMARC\n  (p=quarantine); gunbygunz.com publishes SPF + DMARC (p=none); gunztoken.io publishes SPF (Microsoft\n  365) with no DMARC record; gunzscan.io and gunzchain.io publish neither SPF nor DMARC.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gunzilla-games/refs/heads/main/security/gunzilla-games-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gaming
- Blockchain
- Web3
- EVM
- Avalanche
- JSON-RPC
- GraphQL
- Block Explorer
- NFT
- Video Games
---
