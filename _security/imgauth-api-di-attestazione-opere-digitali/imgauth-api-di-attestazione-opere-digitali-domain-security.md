---
api_specs:
- filename: imgauth-api-di-attestazione-opere-digitali-openapi-original.json
  format: json
  label: imgauth REST API
  slug: imgauth-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imgauth-api-di-attestazione-opere-digitali/refs/heads/main/openapi/imgauth-api-di-attestazione-opere-digitali-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: spaziogenesi.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workers.dev
  spf: true
hosts:
- cert_expires: Oct 24 18:54:24 2026 GMT
  host: imgauth.spaziogenesi.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 17:14:02 2026 GMT
  host: attest-mcp-remote.it-e3f.workers.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imgauth Api Di Attestazione Opere Digitali Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for imgauth — API di attestazione opere digitali, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: imgauth — API di attestazione opere digitali
provider_slug: imgauth-api-di-attestazione-opere-digitali
slug: imgauth-api-di-attestazione-opere-digitali-domain-security
source_filename: imgauth-api-di-attestazione-opere-digitali-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imgauth.spaziogenesi.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 18:54:24 2026 GMT\n  hsts: null\n- host: attest-mcp-remote.it-e3f.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 17:14:02 2026 GMT\n  hsts: false\ndomains:\n- domain: spaziogenesi.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: workers.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imgauth-api-di-attestazione-opere-digitali/refs/heads/main/security/imgauth-api-di-attestazione-opere-digitali-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- digital notarization
- Timestamping
- proof-of-existence
- content authenticity
- Provenance
- Copyright
- IP protection
- Blockchain
- Bitcoin
- OpenTimestamps
- Security
- Document
- E-Signature
- MCP
---
