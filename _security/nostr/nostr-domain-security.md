---
api_specs:
- filename: nostr-asyncapi.yml
  format: yaml
  label: Nostr Protocol (NIP-01)
  slug: nostr-protocol
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nostr/refs/heads/main/asyncapi/nostr-asyncapi.yml
- filename: nostr-asyncapi.yml
  format: yaml
  label: Nostr Relay WebSocket Interface
  slug: relay-interface
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/nostr/refs/heads/main/asyncapi/nostr-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nostr.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: relay.example
  spf: false
hosts:
- cert_expires: Aug 26 10:01:22 2026 GMT
  host: nostr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: relay.example
  https: false
- cert_expires: Aug 14 03:32:50 2026 GMT
  host: www.npmjs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nostr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nostr, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Nostr
provider_slug: nostr
slug: nostr-domain-security
source_filename: nostr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nostr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 10:01:22 2026 GMT\n  hsts: false\n- host: relay.example\n  https: false\n- host: www.npmjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:32:50 2026 GMT\n  hsts: null\ndomains:\n- domain: nostr.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: relay.example\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nostr/refs/heads/main/security/nostr-domain-security.yml
summary_line: TLSv1.3
tags:
- Nostr
- Decentralized Social
- Open Protocol
- Relays
- WebSocket
- Signed Events
- NIP
- Censorship Resistant
- Self-Sovereign Identity
---
