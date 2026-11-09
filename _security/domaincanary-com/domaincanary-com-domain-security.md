---
api_specs:
- filename: domaincanary-com-c-api-openapi.yml
  format: yaml
  label: DomainCanary C API
  slug: domaincanary-com-c-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaincanary-com/openapi/domaincanary-com-c-api-openapi.yml
- filename: domaincanary-com-spf-preflight-api-openapi.yml
  format: yaml
  label: DomainCanary Spf Preflight API
  slug: domaincanary-com-spf-preflight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domaincanary-com/openapi/domaincanary-com-spf-preflight-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: domaincanary.com
  spf: true
hosts:
- cert_expires: Jan 11 19:52:04 2027 GMT
  host: domaincanary.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domaincanary Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DomainCanary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DomainCanary
provider_slug: domaincanary-com
slug: domaincanary-com-domain-security
source_filename: domaincanary-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domaincanary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 19:52:04 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: domaincanary.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/domaincanary-com/security/domaincanary-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DMARC
- Hosted SPF
- Hosted MTA-STS
- MSP Tools
---
