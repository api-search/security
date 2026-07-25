---
api_specs:
- filename: datadome-account-api-openapi.yml
  format: yaml
  label: DataDome Account API
  slug: datadome-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-account-api-openapi.yml
- filename: datadome-accountprotect-api-openapi.yml
  format: yaml
  label: DataDome AccountProtect API
  slug: datadome-accountprotect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-accountprotect-api-openapi.yml
- filename: datadome-customrules-api-openapi.yml
  format: yaml
  label: DataDome CustomRules API
  slug: datadome-customrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-customrules-api-openapi.yml
- filename: datadome-endpoints-api-openapi.yml
  format: yaml
  label: DataDome Endpoints API
  slug: datadome-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-endpoints-api-openapi.yml
- filename: datadome-priorities-api-openapi.yml
  format: yaml
  label: DataDome Priorities API
  slug: datadome-priorities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-priorities-api-openapi.yml
- filename: datadome-templates-api-openapi.yml
  format: yaml
  label: DataDome Templates API
  slug: datadome-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-templates-api-openapi.yml
- filename: datadome-trustedproxies-api-openapi.yml
  format: yaml
  label: DataDome TrustedProxies API
  slug: datadome-trustedproxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-trustedproxies-api-openapi.yml
- filename: datadome-verifiedmodels-api-openapi.yml
  format: yaml
  label: DataDome VerifiedModels API
  slug: datadome-verifiedmodels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/openapi/datadome-verifiedmodels-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datadome.co
  spf: true
hosts:
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: datadome.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 20:09:04 2026 GMT
  host: docs.datadome.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: js.datadome.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datadome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataDome, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DataDome
provider_slug: datadome
slug: datadome-domain-security
source_filename: datadome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datadome.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.datadome.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 20:09:04 2026 GMT\n  hsts: null\n- host: js.datadome.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: datadome.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datadome/refs/heads/main/security/datadome-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bot Mitigation
- Fraud Protection
- Account Protection
- Ad Fraud
- DDoS
- Real-Time
- Edge Security
- Application Security
- Agentic Trust
---
