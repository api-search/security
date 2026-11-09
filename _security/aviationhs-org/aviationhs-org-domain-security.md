---
api_specs:
- filename: aviationhs-org-aircraft-api-openapi.yml
  format: yaml
  label: AviationHS Aircraft API
  slug: aviationhs-org-aircraft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviationhs-org/openapi/aviationhs-org-aircraft-api-openapi.yml
- filename: aviationhs-org-airports-api-openapi.yml
  format: yaml
  label: AviationHS Airports API
  slug: aviationhs-org-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviationhs-org/openapi/aviationhs-org-airports-api-openapi.yml
- filename: aviationhs-org-runway-api-openapi.yml
  format: yaml
  label: AviationHS Runway API
  slug: aviationhs-org-runway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aviationhs-org/openapi/aviationhs-org-runway-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aviationhs.org
  spf: false
hosts:
- cert_expires: Jan 22 13:12:57 2027 GMT
  host: aviationhs.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aviationhs Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AviationHS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AviationHS
provider_slug: aviationhs-org
slug: aviationhs-org-domain-security
source_filename: aviationhs-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aviationhs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 13:12:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aviationhs.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aviationhs-org/security/aviationhs-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Private-Jet
- Charter
- Aviation
- quote-engine
- MCP
---
