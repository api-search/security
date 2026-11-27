---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: microsoft-azure-data-lake-accounts-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Accounts API
  slug: microsoft-azure-data-lake-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-accounts-api-openapi.yml
- filename: microsoft-azure-data-lake-azure-data-lake-storage-rest-api-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Azure Data Lake Storage REST API
  slug: microsoft-azure-data-lake-azure-data-lake-storage-rest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-azure-data-lake-storage-rest-api-api-openapi.yml
- filename: microsoft-azure-data-lake-locations-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Locations API
  slug: microsoft-azure-data-lake-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-locations-api-openapi.yml
- filename: microsoft-azure-data-lake-locationusage-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Location Usage API
  slug: microsoft-azure-data-lake-locationusage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-locationusage-api-openapi.yml
- filename: microsoft-azure-data-lake-operations-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Operations API
  slug: microsoft-azure-data-lake-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-operations-api-openapi.yml
- filename: microsoft-azure-data-lake-trustedidproviders-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Trusted ID Providers API
  slug: microsoft-azure-data-lake-trustedidproviders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-trustedidproviders-api-openapi.yml
- filename: microsoft-azure-data-lake-virtualnetworkrules-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Virtual Network Rules API
  slug: microsoft-azure-data-lake-virtualnetworkrules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-virtualnetworkrules-api-openapi.yml
- filename: microsoft-azure-data-lake-firewall-rules-api-openapi.yml
  format: yaml
  label: Azure Data Lake Storage Firewall Rules API
  slug: microsoft-azure-data-lake-firewall-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-data-lake/openapi/microsoft-azure-data-lake-firewall-rules-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Azure Data Lake Storage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Azure Data Lake Storage secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Azure Data Lake Storage
provider_slug: microsoft-azure-data-lake
scheme_count: 3
schemes:
- description: Shared Key authentication
  in: header
  name: sharedKey
  parameter: Authorization
  sources:
  - openapi/_superseded/microsoft-azure-data-lake-filesystems-api-openapi.yml
  type: apiKey
- description: Shared Access Signature token
  in: query
  name: sasToken
  parameter: sig
  sources:
  - openapi/_superseded/microsoft-azure-data-lake-filesystems-api-openapi.yml
  type: apiKey
- description: Microsoft Entra ID with managed identities to authorize requests against blob, queue, and table data (documented; Microsoft recommends it over Shared Key). Bearer token for resource https://storage.azure.com/.
  documented_only: true
  name: microsoftEntraId
  type: oauth2
slug: microsoft-azure-data-lake-authentication
source_filename: microsoft-azure-data-lake-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://learn.microsoft.com/en-us/rest/api/storageservices/authorize-requests-to-azure-storage\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: sharedKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Shared Key authentication\n  sources:\n  - openapi/_superseded/microsoft-azure-data-lake-filesystems-api-openapi.yml\n- name: sasToken\n  type: apiKey\n  in: query\n  parameter: sig\n  description: Shared Access Signature token\n  sources:\n  - openapi/_superseded/microsoft-azure-data-lake-filesystems-api-openapi.yml\n- name: microsoftEntraId\n  type: oauth2\n  description: Microsoft Entra ID with managed identities to authorize requests against blob, queue, and table data (documented; Microsoft recommends it over Shared Key). Bearer token for resource https://storage.azure.com/.\n  documented_only: true\ndocs: https://learn.microsoft.com/en-us/rest/api/storageservices/authorize-requests-to-azure-storage\n\
  derived_from: openapi/_superseded/microsoft-azure-data-lake-filesystems-api-openapi.yml\nrecommendation: Microsoft Entra ID with managed identities; user delegation SAS when SAS is used.\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-data-lake/authentication/microsoft-azure-data-lake-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Analytics
- Big Data
- Data Lake
- Hierarchical Storage
---
