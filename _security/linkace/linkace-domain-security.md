---
api_specs:
- filename: linkace-bulk-api-openapi.yml
  format: yaml
  label: LinkAce Bulk API
  slug: linkace-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-bulk-api-openapi.yml
- filename: linkace-general-api-openapi.yml
  format: yaml
  label: LinkAce General API
  slug: linkace-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-general-api-openapi.yml
- filename: linkace-links-api-openapi.yml
  format: yaml
  label: LinkAce Links API
  slug: linkace-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-links-api-openapi.yml
- filename: linkace-lists-api-openapi.yml
  format: yaml
  label: LinkAce Lists API
  slug: linkace-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-lists-api-openapi.yml
- filename: linkace-notes-api-openapi.yml
  format: yaml
  label: LinkAce Notes API
  slug: linkace-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-notes-api-openapi.yml
- filename: linkace-search-api-openapi.yml
  format: yaml
  label: LinkAce Search API
  slug: linkace-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-search-api-openapi.yml
- filename: linkace-tags-api-openapi.yml
  format: yaml
  label: LinkAce Tags API
  slug: linkace-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-tags-api-openapi.yml
- filename: linkace-trash-api-openapi.yml
  format: yaml
  label: LinkAce Trash API
  slug: linkace-trash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/linkace/openapi/linkace-trash-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: linkace.org
  spf: true
hosts:
- cert_expires: Jan 11 22:17:40 2027 GMT
  host: linkace.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Linkace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinkAce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: LinkAce
provider_slug: linkace
slug: linkace-domain-security
source_filename: linkace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linkace.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 22:17:40 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: linkace.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/linkace/security/linkace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- OpenSource
- Bookmarking
- SelfHosted
- API
---
