---
api_specs:
- filename: kadena-chainweb-openapi-original.yml
  format: yaml
  label: Kadena Chainweb Node API
  slug: kadena-chainweb-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-chainweb-openapi-original.yml
- filename: kadena-pact-openapi-original.yml
  format: yaml
  label: Kadena Pact REST API
  slug: kadena-pact-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-pact-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kadena.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: chainweb.com
  spf: false
hosts:
- cert_expires: Aug 21 16:00:08 2026 GMT
  host: kadena.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 03:02:25 2026 GMT
  host: docs.kadena.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.chainweb.com
  https: false
kind: domain-security
layout: security
method: probed
name: Kadena Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kadena, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kadena
provider_slug: kadena
slug: kadena-domain-security
source_filename: kadena-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kadena.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 16:00:08 2026 GMT\n  hsts: null\n- host: docs.kadena.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 03:02:25 2026 GMT\n  hsts: null\n- host: api.chainweb.com\n  https: false\ndomains:\n- domain: kadena.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: chainweb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/security/kadena-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto Web3
- Blockchain
- Smart Contracts
- Proof of Work
- Layer 1
- Web3
- Cryptocurrency
- Developer Tools
- Decentralized
---
