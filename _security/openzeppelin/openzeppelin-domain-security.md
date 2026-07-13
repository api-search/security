---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: OpenZeppelin Defender API
  slug: openzeppelin-defender-api
  spec_type: OpenAPI
  url: https://www.api-docs.defender.openzeppelin.com/
- filename: api
  format: yaml
  label: OpenZeppelin Relayer API
  slug: openzeppelin-relayer-api
  spec_type: OpenAPI
  url: https://docs.openzeppelin.com/relayer/1.4.x/api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: openzeppelin.com
  spf: true
hosts:
- cert_expires: Sep 11 13:37:52 2026 GMT
  host: www.openzeppelin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 12:03:53 2026 GMT
  host: docs.openzeppelin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 22:33:55 2026 GMT
  host: defender-api.openzeppelin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openzeppelin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenZeppelin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OpenZeppelin
provider_slug: openzeppelin
slug: openzeppelin-domain-security
source_filename: openzeppelin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openzeppelin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 13:37:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.openzeppelin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 12:03:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: defender-api.openzeppelin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 22:33:55 2026 GMT\n  hsts: null\ndomains:\n- domain: openzeppelin.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openzeppelin/refs/heads/main/security/openzeppelin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Smart Contracts
- Blockchain
- Security
- Ethereum
- DeFi
- Solidity
- Relayer
- Monitoring
- Auditing
---
