---
api_specs:
- filename: ckan-action-api-openapi.yml
  format: yaml
  label: CKAN Action API
  slug: ckan-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ckan/refs/heads/main/openapi/ckan-action-api-openapi.yml
- filename: ckan-ckan-api-api-openapi.yml
  format: yaml
  label: CKAN CKAN API
  slug: ckan-ckan-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ckan/refs/heads/main/openapi/ckan-ckan-api-api-openapi.yml
- filename: ckan-search-api-openapi.yml
  format: yaml
  label: CKAN Search API
  slug: ckan-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ckan/refs/heads/main/openapi/ckan-search-api-openapi.yml
- filename: ckan-solr-api-openapi.yml
  format: yaml
  label: CKAN Solr API
  slug: ckan-solr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ckan/refs/heads/main/openapi/ckan-solr-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ckan.org
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: ckan.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ckan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CKAN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CKAN
provider_slug: ckan
slug: ckan-domain-security
source_filename: ckan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ckan.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ckan.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ckan/refs/heads/main/security/ckan-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Source
- Data-Management
- Government
- Community
---
