---
api_specs:
- filename: amazon-simpledb-action-batchdeleteattributes-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=BatchDeleteAttributes API'
  slug: amazon-simpledb-action-batchdeleteattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-batchdeleteattributes-api-openapi.yml
- filename: amazon-simpledb-action-batchputattributes-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=BatchPutAttributes API'
  slug: amazon-simpledb-action-batchputattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-batchputattributes-api-openapi.yml
- filename: amazon-simpledb-action-createdomain-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=CreateDomain API'
  slug: amazon-simpledb-action-createdomain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-createdomain-api-openapi.yml
- filename: amazon-simpledb-action-deleteattributes-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=DeleteAttributes API'
  slug: amazon-simpledb-action-deleteattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-deleteattributes-api-openapi.yml
- filename: amazon-simpledb-action-deletedomain-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=DeleteDomain API'
  slug: amazon-simpledb-action-deletedomain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-deletedomain-api-openapi.yml
- filename: amazon-simpledb-action-domainmetadata-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=DomainMetadata API'
  slug: amazon-simpledb-action-domainmetadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-domainmetadata-api-openapi.yml
- filename: amazon-simpledb-action-getattributes-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=GetAttributes API'
  slug: amazon-simpledb-action-getattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-getattributes-api-openapi.yml
- filename: amazon-simpledb-action-listdomains-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=ListDomains API'
  slug: amazon-simpledb-action-listdomains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-listdomains-api-openapi.yml
- filename: amazon-simpledb-action-putattributes-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=PutAttributes API'
  slug: amazon-simpledb-action-putattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-putattributes-api-openapi.yml
- filename: amazon-simpledb-action-select-api-openapi.yml
  format: yaml
  label: 'Amazon SimpleDB #Action=Select API'
  slug: amazon-simpledb-action-select-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/openapi/amazon-simpledb-action-select-api-openapi.yml
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
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: sdb.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Simpledb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon SimpleDB, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
slug: amazon-simpledb-domain-security
source_filename: amazon-simpledb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: sdb.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/security/amazon-simpledb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
---
