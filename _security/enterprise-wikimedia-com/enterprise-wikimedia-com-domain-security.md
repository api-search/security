---
api_specs:
- filename: enterprise-wikimedia-com-articles-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Articles API
  slug: enterprise-wikimedia-com-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-articles-api-openapi.yml
- filename: enterprise-wikimedia-com-authentication-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Authentication API
  slug: enterprise-wikimedia-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-authentication-api-openapi.yml
- filename: enterprise-wikimedia-com-batches-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Batches API
  slug: enterprise-wikimedia-com-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-batches-api-openapi.yml
- filename: enterprise-wikimedia-com-codes-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Codes API
  slug: enterprise-wikimedia-com-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-codes-api-openapi.yml
- filename: enterprise-wikimedia-com-languages-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Languages API
  slug: enterprise-wikimedia-com-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-languages-api-openapi.yml
- filename: enterprise-wikimedia-com-namespaces-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Namespaces API
  slug: enterprise-wikimedia-com-namespaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-namespaces-api-openapi.yml
- filename: enterprise-wikimedia-com-projects-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Projects API
  slug: enterprise-wikimedia-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-projects-api-openapi.yml
- filename: enterprise-wikimedia-com-realtime-articles-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Realtime Articles API
  slug: enterprise-wikimedia-com-realtime-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-realtime-articles-api-openapi.yml
- filename: enterprise-wikimedia-com-realtime-wikidata-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Realtime Wikidata API
  slug: enterprise-wikimedia-com-realtime-wikidata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-realtime-wikidata-api-openapi.yml
- filename: enterprise-wikimedia-com-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Snapshots API
  slug: enterprise-wikimedia-com-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-snapshots-api-openapi.yml
- filename: enterprise-wikimedia-com-structured-contents-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Structured Contents API
  slug: enterprise-wikimedia-com-structured-contents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-structured-contents-api-openapi.yml
- filename: enterprise-wikimedia-com-structured-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Structured Snapshots API
  slug: enterprise-wikimedia-com-structured-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-structured-snapshots-api-openapi.yml
- filename: enterprise-wikimedia-com-wikidata-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata API
  slug: enterprise-wikimedia-com-wikidata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-wikidata-api-openapi.yml
- filename: enterprise-wikimedia-com-wikidata-batches-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata Batches API
  slug: enterprise-wikimedia-com-wikidata-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-wikidata-batches-api-openapi.yml
- filename: enterprise-wikimedia-com-wikidata-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia Enterprise Wikidata Snapshots API
  slug: enterprise-wikimedia-com-wikidata-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/enterprise-wikimedia-com/openapi/enterprise-wikimedia-com-wikidata-snapshots-api-openapi.yml
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
  host: auth.enterprise.wikimedia.com
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
provider_slug: enterprise-wikimedia-com
slug: enterprise-wikimedia-com-domain-security
source_filename: enterprise-wikimedia-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: enterprise.wikimedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.enterprise.wikimedia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: null\n- host: auth.enterprise.wikimedia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: wikimedia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/enterprise-wikimedia-com/security/enterprise-wikimedia-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Data
- Enterprise
- Wikimedia
---
