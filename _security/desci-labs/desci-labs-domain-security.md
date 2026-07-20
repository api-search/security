---
api_specs:
- filename: desci-labs-dpid-resolver-openapi.json
  format: json
  label: dPID Resolver API
  slug: dpid-resolver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/desci-labs/refs/heads/main/openapi/desci-labs-dpid-resolver-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dpid.org
  spf: false
hosts:
- cert_expires: Aug 22 16:32:53 2026 GMT
  host: beta.dpid.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 01:59:17 2026 GMT
  host: dev-beta.dpid.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Desci Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeSci Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DeSci Labs
provider_slug: desci-labs
slug: desci-labs-domain-security
source_filename: desci-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beta.dpid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 16:32:53 2026 GMT\n  hsts: null\n- host: dev-beta.dpid.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 01:59:17 2026 GMT\n  hsts: null\ndomains:\n- domain: dpid.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/desci-labs/refs/heads/main/security/desci-labs-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Ai Enterprise Software
- Research Infrastructure
- Decentralized Science
- Scholarly Communication
- Persistent Identifiers
- Open Access
- AI Research Tools
- IPFS
- Model Context Protocol
---
