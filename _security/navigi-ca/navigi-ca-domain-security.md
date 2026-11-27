---
api_specs:
- filename: navigi-ca-communities-api-openapi.yml
  format: yaml
  label: Navigi Communities API
  slug: navigi-ca-communities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/navigi-ca/openapi/navigi-ca-communities-api-openapi.yml
- filename: navigi-ca-export-api-openapi.yml
  format: yaml
  label: Navigi Export API
  slug: navigi-ca-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/navigi-ca/openapi/navigi-ca-export-api-openapi.yml
- filename: navigi-ca-navigi-ca-api-api-openapi.yml
  format: yaml
  label: Navigi Navigi.ca API
  slug: navigi-ca-navigi-ca-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/navigi-ca/openapi/navigi-ca-navigi-ca-api-api-openapi.yml
- filename: navigi-ca-needs-api-openapi.yml
  format: yaml
  label: Navigi Needs API
  slug: navigi-ca-needs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/navigi-ca/openapi/navigi-ca-needs-api-openapi.yml
- filename: navigi-ca-services-api-openapi.yml
  format: yaml
  label: Navigi Services API
  slug: navigi-ca-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/navigi-ca/openapi/navigi-ca-services-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: navigi.ca
  spf: true
hosts:
- cert_expires: Dec 26 20:31:36 2026 GMT
  host: navigi.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Navigi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Navigi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Navigi
provider_slug: navigi-ca
slug: navigi-ca-domain-security
source_filename: navigi-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: navigi.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 20:31:36 2026 GMT\n  hsts: false\ndomains:\n- domain: navigi.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/navigi-ca/security/navigi-ca-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Directory
- Canada
- SocialGood
- Open Data
---
