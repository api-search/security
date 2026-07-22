---
api_specs:
- filename: paxos-v2-openapi-original.json
  format: json
  label: Paxos API v2
  slug: paxos-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paxos/refs/heads/main/openapi/paxos-v2-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paxos.com
  spf: true
hosts:
- cert_expires: Oct 15 15:02:11 2026 GMT
  host: paxos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: api.paxos.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.sandbox.paxos.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paxos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paxos, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paxos
provider_slug: paxos
slug: paxos-domain-security
source_filename: paxos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paxos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 15:02:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.paxos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\n- host: api.sandbox.paxos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: paxos.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paxos/refs/heads/main/security/paxos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Stablecoins
- Cryptocurrency
- Payments
- Crypto Brokerage
- Trading
- Custody
- Blockchain
- Financial Services
- Digital Assets
---
