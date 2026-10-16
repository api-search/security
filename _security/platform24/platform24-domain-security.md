---
api_specs:
- filename: platform24-activities-api-openapi.yml
  format: yaml
  label: Platform24 Activities API
  slug: platform24-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platform24/refs/heads/main/openapi/platform24-activities-api-openapi.yml
- filename: platform24-data-collect-api-openapi.yml
  format: yaml
  label: Platform24 Data Collect API
  slug: platform24-data-collect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platform24/refs/heads/main/openapi/platform24-data-collect-api-openapi.yml
- filename: platform24-front-door-connect-api-openapi.yml
  format: yaml
  label: Platform24 Front Door Connect API
  slug: platform24-front-door-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platform24/refs/heads/main/openapi/platform24-front-door-connect-api-openapi.yml
- filename: platform24-sso-url-api-openapi.yml
  format: yaml
  label: Platform24 Sso Url API
  slug: platform24-sso-url-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platform24/refs/heads/main/openapi/platform24-sso-url-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: platform24.com
  spf: true
hosts:
- cert_expires: Jan  3 11:02:22 2027 GMT
  host: platform24.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Platform24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Platform24, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Platform24
provider_slug: platform24
slug: platform24-domain-security
source_filename: platform24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platform24.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 11:02:22 2027 GMT\n  hsts: false\ndomains:\n- domain: platform24.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/platform24/refs/heads/main/security/platform24-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- DigitalHealth
- Platform
- PatientEngagement
- Company
---
