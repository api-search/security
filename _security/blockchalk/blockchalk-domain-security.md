---
api_specs:
- filename: blockchalk-chalks-api-openapi.yml
  format: yaml
  label: BlockChalk chalks API
  slug: blockchalk-chalks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchalk/refs/heads/main/openapi/blockchalk-chalks-api-openapi.yml
description: ''
domains:
- a_record: false
  caa: []
  created: '2009-07-20'
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: blockchalk.com
  ds: []
  expires: '2028-07-20'
  mx: []
  nameservers:
  - ns1.blockchalk.com
  - ns2.blockchalk.com
  nameservers_responding: false
  registered: true
  registrar: ERANET INTERNATIONAL LIMITED
  soa: false
  spf: false
hosts:
- host: blockchalk.com
  hsts: not-testable
  http_status: 0
  https: false
  resolves: false
  tls: not-testable
- host: www.blockchalk.com
  hsts: not-testable
  http_status: 0
  https: false
  resolves: false
  tls: not-testable
- host: api.blockchalk.com
  hsts: not-testable
  http_status: 0
  https: false
  resolves: false
  tls: not-testable
kind: domain-security
layout: security
method: probed
name: Blockchalk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlockChalk, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BlockChalk
provider_slug: blockchalk
slug: blockchalk-domain-security
source_filename: blockchalk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of blockchalk.com\nname: BlockChalk domain security posture\nsummary: >-\n  blockchalk.com cannot be assessed for transport or email security because it does not\n  resolve. The registration is active (registrar ERANET INTERNATIONAL LIMITED, created\n  2009-07-20, expiring 2028-07-20) and delegates to ns1.blockchalk.com and\n  ns2.blockchalk.com, but those nameservers answer nothing, so every record type below comes\n  back empty and no TLS handshake is possible. This is the expected result for a retired\n  service, not a misconfiguration finding against a live provider.\nhosts:\n- host: blockchalk.com\n  resolves: false\n  https: false\n  http_status: 000\n  tls: not-testable\n  hsts: not-testable\n- host: www.blockchalk.com\n  resolves: false\n  https: false\n  http_status: 000\n  tls: not-testable\n  hsts: not-testable\n- host: api.blockchalk.com\n  resolves: false\n  https: false\n  http_status: 000\n\
  \  tls: not-testable\n  hsts: not-testable\ndomains:\n- domain: blockchalk.com\n  registered: true\n  registrar: ERANET INTERNATIONAL LIMITED\n  created: '2009-07-20'\n  expires: '2028-07-20'\n  nameservers:\n  - ns1.blockchalk.com\n  - ns2.blockchalk.com\n  nameservers_responding: false\n  a_record: false\n  soa: false\n  dnssec: false\n  ds: []\n  caa: []\n  mx: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\nnotes: >-\n  An earlier automated pass attributed web.archive.org and archive.org results to this\n  provider because the only reachable humanURL in apis.yml is a Wayback Machine link. That\n  attribution was incorrect and has been removed; nothing in this file describes any host\n  other than BlockChalk's own.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockchalk/refs/heads/main/security/blockchalk-domain-security.yml
summary_line: HSTS
tags:
- Company
- Location
- Geolocation
- Social
- Messaging
- Local
- Neighborhood
- Mobile
- Retired
---
