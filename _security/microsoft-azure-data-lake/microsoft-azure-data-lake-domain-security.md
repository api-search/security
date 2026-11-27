---
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
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
hosts:
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
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
name: Azure Data Lake Storage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Data Lake Storage, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Data Lake Storage
provider_slug: microsoft-azure-data-lake
slug: microsoft-azure-data-lake-domain-security
source_filename: microsoft-azure-data-lake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-data-lake/security/microsoft-azure-data-lake-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Big Data
- Data Lake
- Hierarchical Storage
---
