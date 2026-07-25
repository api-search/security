---
api_specs:
- filename: amazon-memorydb-acls-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB ACLs API
  slug: amazon-memorydb-acls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-acls-api-openapi.yml
- filename: amazon-memorydb-clusters-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB Clusters API
  slug: amazon-memorydb-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-clusters-api-openapi.yml
- filename: amazon-memorydb-engineversions-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB EngineVersions API
  slug: amazon-memorydb-engineversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-engineversions-api-openapi.yml
- filename: amazon-memorydb-events-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB Events API
  slug: amazon-memorydb-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-events-api-openapi.yml
- filename: amazon-memorydb-nodetypes-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB NodeTypes API
  slug: amazon-memorydb-nodetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-nodetypes-api-openapi.yml
- filename: amazon-memorydb-parametergroups-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB ParameterGroups API
  slug: amazon-memorydb-parametergroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-parametergroups-api-openapi.yml
- filename: amazon-memorydb-reservednodes-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB ReservedNodes API
  slug: amazon-memorydb-reservednodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-reservednodes-api-openapi.yml
- filename: amazon-memorydb-shards-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB Shards API
  slug: amazon-memorydb-shards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-shards-api-openapi.yml
- filename: amazon-memorydb-snapshots-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB Snapshots API
  slug: amazon-memorydb-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-snapshots-api-openapi.yml
- filename: amazon-memorydb-subnetgroups-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB SubnetGroups API
  slug: amazon-memorydb-subnetgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-subnetgroups-api-openapi.yml
- filename: amazon-memorydb-tags-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB Tags API
  slug: amazon-memorydb-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-tags-api-openapi.yml
- filename: amazon-memorydb-users-api-openapi.yml
  format: yaml
  label: Amazon MemoryDB Users API
  slug: amazon-memorydb-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/openapi/amazon-memorydb-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: memory-db.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: memory-db.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Memorydb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon MemoryDB, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon MemoryDB
provider_slug: amazon-memorydb
slug: amazon-memorydb-domain-security
source_filename: amazon-memorydb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: memory-db.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\n- host: memory-db.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/security/amazon-memorydb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Broadcasting
- Media Processing
- Media
---
