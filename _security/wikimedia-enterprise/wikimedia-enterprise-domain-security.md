---
api_specs:
- filename: wikimedia-enterprise-articles-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Articles API
  slug: wikimedia-enterprise-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-articles-api-openapi.yml
- filename: wikimedia-enterprise-authentication-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Authentication API
  slug: wikimedia-enterprise-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-authentication-api-openapi.yml
- filename: wikimedia-enterprise-batches-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Batches API
  slug: wikimedia-enterprise-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-batches-api-openapi.yml
- filename: wikimedia-enterprise-codes-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Codes API
  slug: wikimedia-enterprise-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-codes-api-openapi.yml
- filename: wikimedia-enterprise-languages-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Languages API
  slug: wikimedia-enterprise-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-languages-api-openapi.yml
- filename: wikimedia-enterprise-namespaces-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Namespaces API
  slug: wikimedia-enterprise-namespaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-namespaces-api-openapi.yml
- filename: wikimedia-enterprise-projects-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Projects API
  slug: wikimedia-enterprise-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-projects-api-openapi.yml
- filename: wikimedia-enterprise-realtime-articles-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Realtime Articles API
  slug: wikimedia-enterprise-realtime-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-realtime-articles-api-openapi.yml
- filename: wikimedia-enterprise-realtime-wikidata-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Realtime Wikidata API
  slug: wikimedia-enterprise-realtime-wikidata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-realtime-wikidata-api-openapi.yml
- filename: wikimedia-enterprise-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Snapshots API
  slug: wikimedia-enterprise-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-snapshots-api-openapi.yml
- filename: wikimedia-enterprise-structured-contents-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Structured Contents API
  slug: wikimedia-enterprise-structured-contents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-structured-contents-api-openapi.yml
- filename: wikimedia-enterprise-structured-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Structured Snapshots API
  slug: wikimedia-enterprise-structured-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-structured-snapshots-api-openapi.yml
- filename: wikimedia-enterprise-wikidata-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata API
  slug: wikimedia-enterprise-wikidata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-wikidata-api-openapi.yml
- filename: wikimedia-enterprise-wikidata-batches-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata Batches API
  slug: wikimedia-enterprise-wikidata-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-wikidata-batches-api-openapi.yml
- filename: wikimedia-enterprise-wikidata-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata Snapshots API
  slug: wikimedia-enterprise-wikidata-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wikimedia-enterprise/openapi/wikimedia-enterprise-wikidata-snapshots-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wikimedia.com
  spf: true
hosts:
- cert_expires: Mar 30 23:59:59 2027 GMT
  host: enterprise.wikimedia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: api.enterprise.wikimedia.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: realtime.enterprise.wikimedia.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Wikimedia Enterprise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wikimedia Enterprise, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Wikimedia Enterprise
provider_slug: wikimedia-enterprise
slug: wikimedia-enterprise-domain-security
source_filename: wikimedia-enterprise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enterprise.wikimedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.enterprise.wikimedia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: null\n- host: realtime.enterprise.wikimedia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: wikimedia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/wikimedia-enterprise/security/wikimedia-enterprise-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Wikipedia
- wikidata
- Open Knowledge
- Datasets
- Content
- Knowledge Graph
- Streaming
- AI Training Data
---
