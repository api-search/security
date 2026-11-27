---
api_specs:
- filename: dane-biznes-gov-pl-public-fbc-service-descriptions-controller-api-openapi.yml
  format: yaml
  label: Hurtownia danych CEIDG i Biznes.gov.pl Public Fbc Service Descriptions Controller API
  slug: dane-biznes-gov-pl-public-fbc-service-descriptions-controller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dane-biznes-gov-pl/openapi/dane-biznes-gov-pl-public-fbc-service-descriptions-controller-api-openapi.yml
- filename: dane-biznes-gov-pl-resource-api-openapi.yml
  format: yaml
  label: Hurtownia danych CEIDG i Biznes.gov.pl Resource API
  slug: dane-biznes-gov-pl-resource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dane-biznes-gov-pl/openapi/dane-biznes-gov-pl-resource-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: biznes.gov.pl
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: dane.biznes.gov.pl
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hurtownia danych CEIDG i Biznes.gov.pl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hurtownia danych CEIDG i Biznes.gov.pl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hurtownia danych CEIDG i Biznes.gov.pl
provider_slug: dane-biznes-gov-pl
slug: dane-biznes-gov-pl-domain-security
source_filename: dane-biznes-gov-pl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dane.biznes.gov.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: biznes.gov.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dane-biznes-gov-pl/security/dane-biznes-gov-pl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Business Registry
- Open Data
- Poland
- Companies
- Public Sector
---
