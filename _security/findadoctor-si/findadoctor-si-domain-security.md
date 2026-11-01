---
api_specs:
- filename: findadoctor-si-about-api-openapi.yml
  format: yaml
  label: findadoctor-si About API
  slug: findadoctor-si-about-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-about-api-openapi.yml
- filename: findadoctor-si-doctors-api-openapi.yml
  format: yaml
  label: findadoctor-si Doctors API
  slug: findadoctor-si-doctors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-doctors-api-openapi.yml
- filename: findadoctor-si-gp-practices-api-openapi.yml
  format: yaml
  label: findadoctor-si Gp Practices API
  slug: findadoctor-si-gp-practices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-gp-practices-api-openapi.yml
- filename: findadoctor-si-procedure-volumes-api-openapi.yml
  format: yaml
  label: findadoctor-si Procedure Volumes API
  slug: findadoctor-si-procedure-volumes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-procedure-volumes-api-openapi.yml
- filename: findadoctor-si-procedures-api-openapi.yml
  format: yaml
  label: findadoctor-si Procedures API
  slug: findadoctor-si-procedures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-procedures-api-openapi.yml
- filename: findadoctor-si-search-api-openapi.yml
  format: yaml
  label: findadoctor-si Search API
  slug: findadoctor-si-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-search-api-openapi.yml
- filename: findadoctor-si-specialties-api-openapi.yml
  format: yaml
  label: findadoctor-si Specialties API
  slug: findadoctor-si-specialties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-specialties-api-openapi.yml
- filename: findadoctor-si-terms-api-openapi.yml
  format: yaml
  label: findadoctor-si Terms API
  slug: findadoctor-si-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-terms-api-openapi.yml
- filename: findadoctor-si-waitlist-api-openapi.yml
  format: yaml
  label: findadoctor-si Waitlist API
  slug: findadoctor-si-waitlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findadoctor-si/openapi/findadoctor-si-waitlist-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: findadoctor.si
  spf: true
hosts:
- cert_expires: Jan 10 15:55:35 2027 GMT
  host: findadoctor.si
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Findadoctor Si Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for findadoctor-si, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: findadoctor-si
provider_slug: findadoctor-si
slug: findadoctor-si-domain-security
source_filename: findadoctor-si-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: findadoctor.si\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 15:55:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: findadoctor.si\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/findadoctor-si/security/findadoctor-si-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Data
- AI
- Doctor
- International
---
