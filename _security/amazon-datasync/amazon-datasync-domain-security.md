---
api_specs:
- filename: amazon-datasync-amazon-datasync-rest-api-api-openapi.yml
  format: yaml
  label: Amazon DataSync Amazon DataSync REST API
  slug: amazon-datasync-amazon-datasync-rest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-amazon-datasync-rest-api-api-openapi.yml
- filename: amazon-datasync-agent-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Agent API
  slug: amazon-datasync-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-agent-api-openapi.yml
- filename: amazon-datasync-location-azure-blob-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Azure Blob API
  slug: amazon-datasync-location-azure-blob-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-azure-blob-api-openapi.yml
- filename: amazon-datasync-location-ef-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Ef API
  slug: amazon-datasync-location-ef-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-ef-api-openapi.yml
- filename: amazon-datasync-location-fsx-lustre-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Fsx Lustre API
  slug: amazon-datasync-location-fsx-lustre-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-fsx-lustre-api-openapi.yml
- filename: amazon-datasync-location-fsx-ontap-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Fsx Ontap API
  slug: amazon-datasync-location-fsx-ontap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-fsx-ontap-api-openapi.yml
- filename: amazon-datasync-location-fsx-open-zf-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Fsx Open Zf API
  slug: amazon-datasync-location-fsx-open-zf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-fsx-open-zf-api-openapi.yml
- filename: amazon-datasync-location-fsx-window-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Fsx Window API
  slug: amazon-datasync-location-fsx-window-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-fsx-window-api-openapi.yml
- filename: amazon-datasync-location-hdf-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Hdf API
  slug: amazon-datasync-location-hdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-hdf-api-openapi.yml
- filename: amazon-datasync-location-nf-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Nf API
  slug: amazon-datasync-location-nf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-nf-api-openapi.yml
- filename: amazon-datasync-location-object-storage-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Object Storage API
  slug: amazon-datasync-location-object-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-object-storage-api-openapi.yml
- filename: amazon-datasync-location-smb-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Location Smb API
  slug: amazon-datasync-location-smb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-location-smb-api-openapi.yml
- filename: amazon-datasync-operations-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Operations API
  slug: amazon-datasync-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-operations-api-openapi.yml
- filename: amazon-datasync-task-execution-api-openapi.yml
  format: yaml
  label: Amazon DataSync Datasync Task Execution API
  slug: amazon-datasync-task-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-datasync/openapi/amazon-datasync-task-execution-api-openapi.yml
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
- host: datasync.amazonaws.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon Datasync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon DataSync, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon DataSync
provider_slug: amazon-datasync
slug: amazon-datasync-domain-security
source_filename: amazon-datasync-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: datasync.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-datasync/security/amazon-datasync-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
---
