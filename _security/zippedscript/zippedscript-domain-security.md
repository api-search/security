---
api_specs:
- filename: zippedscript-authentication-api-openapi.yml
  format: yaml
  label: ZippedScript Authentication API
  slug: zippedscript-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-authentication-api-openapi.yml
- filename: zippedscript-direct-api-openapi.yml
  format: yaml
  label: ZippedScript Direct API
  slug: zippedscript-direct-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-direct-api-openapi.yml
- filename: zippedscript-employment-api-openapi.yml
  format: yaml
  label: ZippedScript Employment API
  slug: zippedscript-employment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-employment-api-openapi.yml
- filename: zippedscript-institution-api-openapi.yml
  format: yaml
  label: ZippedScript Institution API
  slug: zippedscript-institution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-institution-api-openapi.yml
- filename: zippedscript-reference-checks-api-openapi.yml
  format: yaml
  label: ZippedScript Reference Checks API
  slug: zippedscript-reference-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-reference-checks-api-openapi.yml
- filename: zippedscript-user-api-openapi.yml
  format: yaml
  label: ZippedScript User API
  slug: zippedscript-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-user-api-openapi.yml
- filename: zippedscript-verification-api-openapi.yml
  format: yaml
  label: ZippedScript Verification API
  slug: zippedscript-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zippedscript/openapi/zippedscript-verification-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zippedscript.com
  spf: true
hosts:
- cert_expires: Nov 16 21:11:47 2026 GMT
  host: www.zippedscript.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zippedscript Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZippedScript, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ZippedScript
provider_slug: zippedscript
slug: zippedscript-domain-security
source_filename: zippedscript-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zippedscript.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 21:11:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zippedscript.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/zippedscript/security/zippedscript-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Education
- Verification
- SaaS
- Background-Check
---
