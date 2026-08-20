---
api_specs:
- filename: solr-collections-api-openapi.yml
  format: yaml
  label: Apache Solr Collections API
  slug: solr-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solr/refs/heads/main/openapi/solr-collections-api-openapi.yml
- filename: solr-collectionsadminhandler-api-openapi.yml
  format: yaml
  label: Apache Solr CollectionsAdminHandler API
  slug: solr-collectionsadminhandler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solr/refs/heads/main/openapi/solr-collectionsadminhandler-api-openapi.yml
- filename: solr-config-api-openapi.yml
  format: yaml
  label: Apache Solr Config API
  slug: solr-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solr/refs/heads/main/openapi/solr-config-api-openapi.yml
- filename: solr-cores-api-openapi.yml
  format: yaml
  label: Apache Solr Cores API
  slug: solr-cores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solr/refs/heads/main/openapi/solr-cores-api-openapi.yml
- filename: solr-schema-api-openapi.yml
  format: yaml
  label: Apache Solr Schema API
  slug: solr-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solr/refs/heads/main/openapi/solr-schema-api-openapi.yml
- filename: solr-shards-api-openapi.yml
  format: yaml
  label: Apache Solr Shards API
  slug: solr-shards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solr/refs/heads/main/openapi/solr-shards-api-openapi.yml
- filename: solr-update-api-openapi.yml
  format: yaml
  label: Apache Solr Update API
  slug: solr-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solr/refs/heads/main/openapi/solr-update-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: solr.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Solr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Solr
provider_slug: solr
slug: solr-domain-security
source_filename: solr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: solr.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solr/refs/heads/main/security/solr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Enterprise Search
- Full-Text Search
- Open-Source
- Lucene
- Indexing
---
