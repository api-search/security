---
api_key_in: []
api_specs:
- filename: oracle-console-connections-api-openapi.yml
  format: yaml
  label: Oracle Console Connections API
  slug: oracle-console-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/openapi/oracle-console-connections-api-openapi.yml
- filename: oracle-images-api-openapi.yml
  format: yaml
  label: Oracle Images API
  slug: oracle-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/openapi/oracle-images-api-openapi.yml
- filename: oracle-instances-api-openapi.yml
  format: yaml
  label: Oracle Instances API
  slug: oracle-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/openapi/oracle-instances-api-openapi.yml
- filename: oracle-shapes-api-openapi.yml
  format: yaml
  label: Oracle Shapes API
  slug: oracle-shapes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/openapi/oracle-shapes-api-openapi.yml
- filename: oracle-vnic-attachments-api-openapi.yml
  format: yaml
  label: Oracle VNIC Attachments API
  slug: oracle-vnic-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/openapi/oracle-vnic-attachments-api-openapi.yml
- filename: oracle-volume-attachments-api-openapi.yml
  format: yaml
  label: Oracle Volume Attachments API
  slug: oracle-volume-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/openapi/oracle-volume-attachments-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oracle
provider_slug: oracle
scheme_count: 1
schemes:
- description: OCI uses a custom request signing scheme based on RSA key pairs. Each API request must include an Authorization header with the signature computed from the request headers, method, and path. See https://docs.oracle.com/en-us/iaas/Content/API/Concepts/signingrequests.htm
  name: ociRequestSigning
  scheme: bearer
  sources:
  - openapi/oci-compute-api-openapi.yml
  type: http
slug: oracle-authentication
source_filename: oracle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oci-compute-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ociRequestSigning\n  type: http\n  scheme: bearer\n  description: OCI uses a custom request signing scheme based on RSA key pairs. Each API request\n    must include an Authorization header with the signature computed from the request headers,\n    method, and path. See https://docs.oracle.com/en-us/iaas/Content/API/Concepts/signingrequests.htm\n  sources:\n  - openapi/oci-compute-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/authentication/oracle-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
- Fortune 100
---
