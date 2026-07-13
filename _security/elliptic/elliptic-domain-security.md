---
api_specs:
- filename: aml-api-oauth.json
  format: json
  label: Elliptic AML API
  slug: elliptic-aml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/aml-api-oauth.json
- filename: ia-api.json
  format: json
  label: Elliptic AI API
  slug: elliptic-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/ia-api.json
- filename: sanctions-api.json
  format: json
  label: Elliptic Sanctions API
  slug: elliptic-sanctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/sanctions-api.json
- filename: data-fabric.yaml
  format: yaml
  label: Elliptic Data Fabric API
  slug: elliptic-data-fabric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/openapi/data-fabric.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: elliptic.co
  spf: true
hosts:
- cert_expires: Sep 11 18:42:23 2026 GMT
  host: developers.elliptic.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: aml-api.elliptic.co
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: sanctions-api.elliptic.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Elliptic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elliptic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Elliptic
provider_slug: elliptic
slug: elliptic-domain-security
source_filename: elliptic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.elliptic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:42:23 2026 GMT\n  hsts: null\n- host: aml-api.elliptic.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: null\n- host: sanctions-api.elliptic.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: elliptic.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elliptic/refs/heads/main/security/elliptic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Blockchain
- Crypto
- Compliance
- AML
- Transaction Screening
- Wallet Screening
- Risk Scoring
- Analytics
---
