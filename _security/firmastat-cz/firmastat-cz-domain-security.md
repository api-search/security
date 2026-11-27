---
api_specs:
- filename: firmastat-cz-firma-api-openapi.yml
  format: yaml
  label: Firmastat Firma API
  slug: firmastat-cz-firma-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-firma-api-openapi.yml
- filename: firmastat-cz-firmy-api-openapi.yml
  format: yaml
  label: Firmastat Firmy API
  slug: firmastat-cz-firmy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-firmy-api-openapi.yml
- filename: firmastat-cz-health-api-openapi.yml
  format: yaml
  label: Firmastat Health API
  slug: firmastat-cz-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-health-api-openapi.yml
- filename: firmastat-cz-osoba-api-openapi.yml
  format: yaml
  label: Firmastat Osoba API
  slug: firmastat-cz-osoba-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-osoba-api-openapi.yml
- filename: firmastat-cz-osoby-api-openapi.yml
  format: yaml
  label: Firmastat Osoby API
  slug: firmastat-cz-osoby-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-osoby-api-openapi.yml
- filename: firmastat-cz-suggest-api-openapi.yml
  format: yaml
  label: Firmastat Suggest API
  slug: firmastat-cz-suggest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-suggest-api-openapi.yml
- filename: firmastat-cz-vyhledavani-api-openapi.yml
  format: yaml
  label: Firmastat Vyhledavani API
  slug: firmastat-cz-vyhledavani-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-vyhledavani-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: firmastat.cz
  spf: true
hosts:
- cert_expires: Jan 27 04:19:05 2027 GMT
  host: firmastat.cz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firmastat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firmastat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Firmastat
provider_slug: firmastat-cz
slug: firmastat-cz-domain-security
source_filename: firmastat-cz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firmastat.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 04:19:05 2027 GMT\n  hsts: false\ndomains:\n- domain: firmastat.cz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/firmastat-cz/security/firmastat-cz-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Czech
- Business
- Data
- Search
---
