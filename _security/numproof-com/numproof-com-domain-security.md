---
api_specs:
- filename: numproof-com-api-openapi.json
  format: json
  label: NumProof Api API
  slug: numproof-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numproof-com/openapi/_original/numproof-com-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: numproof.com
  spf: true
hosts:
- cert_expires: Jan  9 04:50:23 2027 GMT
  host: numproof.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NumProof Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NumProof, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NumProof
provider_slug: numproof-com
slug: numproof-com-domain-security
source_filename: numproof-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numproof.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 04:50:23 2027 GMT\n  hsts: false\ndomains:\n- domain: numproof.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/numproof-com/security/numproof-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Finance
- Verification
- Zero Trust
---
