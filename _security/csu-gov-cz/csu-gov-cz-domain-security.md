---
api_specs:
- filename: csu-gov-cz-administrace-api-openapi.yml
  format: yaml
  label: Czech Statistical Office (CZSO) Administrace API
  slug: csu-gov-cz-administrace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csu-gov-cz/openapi/csu-gov-cz-administrace-api-openapi.yml
- filename: csu-gov-cz-data-api-openapi.yml
  format: yaml
  label: Czech Statistical Office (CZSO) Data API
  slug: csu-gov-cz-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csu-gov-cz/openapi/csu-gov-cz-data-api-openapi.yml
- filename: csu-gov-cz-dimenze-api-openapi.yml
  format: yaml
  label: Czech Statistical Office (CZSO) Dimenze API
  slug: csu-gov-cz-dimenze-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csu-gov-cz/openapi/csu-gov-cz-dimenze-api-openapi.yml
- filename: csu-gov-cz-katalog-api-openapi.yml
  format: yaml
  label: Czech Statistical Office (CZSO) Katalog API
  slug: csu-gov-cz-katalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csu-gov-cz/openapi/csu-gov-cz-katalog-api-openapi.yml
- filename: csu-gov-cz-metadata-api-openapi.yml
  format: yaml
  label: Czech Statistical Office (CZSO) Metadata API
  slug: csu-gov-cz-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csu-gov-cz/openapi/csu-gov-cz-metadata-api-openapi.yml
- filename: csu-gov-cz-sady-api-openapi.yml
  format: yaml
  label: Czech Statistical Office (CZSO) Sady API
  slug: csu-gov-cz-sady-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csu-gov-cz/openapi/csu-gov-cz-sady-api-openapi.yml
- filename: csu-gov-cz-ukazatele-api-openapi.yml
  format: yaml
  label: Czech Statistical Office (CZSO) Ukazatele API
  slug: csu-gov-cz-ukazatele-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csu-gov-cz/openapi/csu-gov-cz-ukazatele-api-openapi.yml
- filename: csu-gov-cz-velikosti-api-openapi.yml
  format: yaml
  label: Czech Statistical Office (CZSO) Velikosti API
  slug: csu-gov-cz-velikosti-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csu-gov-cz/openapi/csu-gov-cz-velikosti-api-openapi.yml
- filename: csu-gov-cz-vybery-api-openapi.yml
  format: yaml
  label: Czech Statistical Office (CZSO) Vybery API
  slug: csu-gov-cz-vybery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/csu-gov-cz/openapi/csu-gov-cz-vybery-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: csu.gov.cz
  spf: true
hosts:
- cert_expires: Jan 23 10:02:57 2027 GMT
  host: csu.gov.cz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Czech Statistical Office (CZSO) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Czech Statistical Office (CZSO), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Czech Statistical Office (CZSO)
provider_slug: csu-gov-cz
slug: csu-gov-cz-domain-security
source_filename: csu-gov-cz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: csu.gov.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 10:02:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: csu.gov.cz\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/csu-gov-cz/security/csu-gov-cz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Statistics
- Open Data
- Czech Republic
- JSON-stat
- Public Sector
---
