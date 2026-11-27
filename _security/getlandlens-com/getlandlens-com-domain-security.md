---
api_specs:
- filename: getlandlens-com-colleges-api-openapi.yml
  format: yaml
  label: LandLens Colleges API
  slug: getlandlens-com-colleges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlandlens-com/openapi/getlandlens-com-colleges-api-openapi.yml
- filename: getlandlens-com-landlords-api-openapi.yml
  format: yaml
  label: LandLens Landlords API
  slug: getlandlens-com-landlords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlandlens-com/openapi/getlandlens-com-landlords-api-openapi.yml
- filename: getlandlens-com-properties-api-openapi.yml
  format: yaml
  label: LandLens Properties API
  slug: getlandlens-com-properties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlandlens-com/openapi/getlandlens-com-properties-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getlandlens.com
  spf: true
hosts:
- cert_expires: Feb  3 06:08:58 2027 GMT
  host: getlandlens.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LandLens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LandLens, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LandLens
provider_slug: getlandlens-com
slug: getlandlens-com-domain-security
source_filename: getlandlens-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getlandlens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 06:08:58 2027 GMT\n  hsts: false\ndomains:\n- domain: getlandlens.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getlandlens-com/security/getlandlens-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Student Housing
- Data Platform
- Reviews
---
