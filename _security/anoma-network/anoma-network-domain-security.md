---
api_specs:
- filename: anoma-network-openapi-generated.yml
  format: yaml
  label: Anoma Network API
  slug: anoma-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anoma-network/refs/heads/main/openapi/_ae-authored/anoma-network-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: anoma.net
  spf: true
hosts:
- cert_expires: Nov 11 18:34:05 2026 GMT
  host: anoma.net
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anoma Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anoma Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Anoma Network
provider_slug: anoma-network
slug: anoma-network-domain-security
source_filename: anoma-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anoma.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 18:34:05 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: anoma.net\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anoma-network/refs/heads/main/security/anoma-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Decentralized
- Operating System
- SDK
- Interoperability
---
