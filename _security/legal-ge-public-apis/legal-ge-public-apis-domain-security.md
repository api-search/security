---
api_specs:
- filename: legal-ge-public-apis-directory-api-openapi.yml
  format: yaml
  label: legal.ge Public APIs Directory API
  slug: legal-ge-public-apis-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/legal-ge-public-apis/refs/heads/main/openapi/legal-ge-public-apis-directory-api-openapi.yml
- filename: legal-ge-public-apis-matching-api-openapi.yml
  format: yaml
  label: legal.ge Public APIs Matching API
  slug: legal-ge-public-apis-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/legal-ge-public-apis/refs/heads/main/openapi/legal-ge-public-apis-matching-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: legal.ge
  spf: true
hosts:
- cert_expires: Oct  9 03:51:38 2026 GMT
  host: legal.ge
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Legal Ge Public Apis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for legal.ge Public APIs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: legal.ge Public APIs
provider_slug: legal-ge-public-apis
slug: legal-ge-public-apis-domain-security
source_filename: legal-ge-public-apis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: legal.ge\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 03:51:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: legal.ge\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legal-ge-public-apis/refs/heads/main/security/legal-ge-public-apis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- law
- legal-services
- Directory
- georgia
- AI Agents
- MCP
- specialists
- professional-services
- Marketplace
- multilingual
- legal-tech
---
