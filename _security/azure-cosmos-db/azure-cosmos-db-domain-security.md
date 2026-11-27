---
api_specs:
- filename: azure-cosmos-db-datatransfer-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Data Transfer API
  slug: azure-cosmos-db-datatransfer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-datatransfer-api-openapi.yml
- filename: azure-cosmos-db-fleets-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Fleets API
  slug: azure-cosmos-db-fleets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-fleets-api-openapi.yml
- filename: azure-cosmos-db-graphapicompute-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Graph API Compute API
  slug: azure-cosmos-db-graphapicompute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-graphapicompute-api-openapi.yml
- filename: azure-cosmos-db-materializedviewsbuilder-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Materialized Views Builder API
  slug: azure-cosmos-db-materializedviewsbuilder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-materializedviewsbuilder-api-openapi.yml
- filename: azure-cosmos-db-notebookworkspacesresource-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Notebook Workspaces Resource API
  slug: azure-cosmos-db-notebookworkspacesresource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-notebookworkspacesresource-api-openapi.yml
- filename: azure-cosmos-db-operations-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Operations API
  slug: azure-cosmos-db-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-operations-api-openapi.yml
- filename: azure-cosmos-db-privatelinkresources-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Private Link Resources API
  slug: azure-cosmos-db-privatelinkresources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-privatelinkresources-api-openapi.yml
- filename: azure-cosmos-db-providers-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Providers API
  slug: azure-cosmos-db-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-providers-api-openapi.yml
- filename: azure-cosmos-db-sqldedicatedgateway-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Sql Dedicated Gateway API
  slug: azure-cosmos-db-sqldedicatedgateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-sqldedicatedgateway-api-openapi.yml
- filename: azure-cosmos-db-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Subscriptions API
  slug: azure-cosmos-db-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-subscriptions-api-openapi.yml
- filename: azure-cosmos-db-private-endpoint-connections-api-openapi.yml
  format: yaml
  label: Azure Cosmos DB Private Endpoint Connections API
  slug: azure-cosmos-db-private-endpoint-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/azure-cosmos-db/openapi/azure-cosmos-db-private-endpoint-connections-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 19:05:38 2027 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Azure Cosmos DB Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Cosmos DB, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Cosmos DB
provider_slug: azure-cosmos-db
slug: azure-cosmos-db-domain-security
source_filename: azure-cosmos-db-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 19:05:38 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/azure-cosmos-db/security/azure-cosmos-db-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- NoSQL
- Document Database
- Vector Search
- Globally Distributed
- Cloud
- Microsoft Azure
---
