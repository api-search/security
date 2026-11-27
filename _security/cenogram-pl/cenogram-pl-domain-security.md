---
api_specs:
- filename: cenogram-pl-demographics-api-openapi.yml
  format: yaml
  label: Cenogram Demographics API
  slug: cenogram-pl-demographics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-demographics-api-openapi.yml
- filename: cenogram-pl-infrastructure-api-openapi.yml
  format: yaml
  label: Cenogram Infrastructure API
  slug: cenogram-pl-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-infrastructure-api-openapi.yml
- filename: cenogram-pl-locations-api-openapi.yml
  format: yaml
  label: Cenogram Locations API
  slug: cenogram-pl-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-locations-api-openapi.yml
- filename: cenogram-pl-parcels-api-openapi.yml
  format: yaml
  label: Cenogram Parcels API
  slug: cenogram-pl-parcels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-parcels-api-openapi.yml
- filename: cenogram-pl-spatial-api-openapi.yml
  format: yaml
  label: Cenogram Spatial API
  slug: cenogram-pl-spatial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-spatial-api-openapi.yml
- filename: cenogram-pl-statistics-api-openapi.yml
  format: yaml
  label: Cenogram Statistics API
  slug: cenogram-pl-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-statistics-api-openapi.yml
- filename: cenogram-pl-transactions-api-openapi.yml
  format: yaml
  label: Cenogram Transactions API
  slug: cenogram-pl-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cenogram-pl/openapi/cenogram-pl-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cenogram.pl
  spf: true
hosts:
- cert_expires: Dec 10 13:50:45 2026 GMT
  host: cenogram.pl
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cenogram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cenogram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cenogram
provider_slug: cenogram-pl
slug: cenogram-pl-domain-security
source_filename: cenogram-pl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cenogram.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 13:50:45 2026 GMT\n  hsts: false\ndomains:\n- domain: cenogram.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cenogram-pl/security/cenogram-pl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Data
- Analytics
- Poland
---
