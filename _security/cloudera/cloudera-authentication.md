---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: cloudera-audit-openapi.yml
  format: yaml
  label: Cloudera Audit Service API
  slug: cloudera-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-audit-openapi.yml
- filename: cloudera-cloudprivatelinks-openapi.yml
  format: yaml
  label: Cloudera Private Links API
  slug: cloudera-cloudprivatelinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-cloudprivatelinks-openapi.yml
- filename: cloudera-compute-openapi.yml
  format: yaml
  label: Cloudera Compute Service API
  slug: cloudera-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-compute-openapi.yml
- filename: cloudera-consumption-openapi.yml
  format: yaml
  label: Cloudera Consumption API
  slug: cloudera-consumption-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-consumption-openapi.yml
- filename: cloudera-datacatalog-openapi.yml
  format: yaml
  label: Cloudera Data Catalog API
  slug: cloudera-datacatalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-datacatalog-openapi.yml
- filename: cloudera-datahub-openapi.yml
  format: yaml
  label: Cloudera Data Hub API
  slug: cloudera-datahub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-datahub-openapi.yml
- filename: cloudera-datalake-openapi.yml
  format: yaml
  label: Cloudera Datalake API
  slug: cloudera-datalake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-datalake-openapi.yml
- filename: cloudera-de-openapi.yml
  format: yaml
  label: Cloudera Data Engineering API
  slug: cloudera-dataengineering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-de-openapi.yml
- filename: cloudera-df-openapi.yml
  format: yaml
  label: Cloudera DataFlow API
  slug: cloudera-dataflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-df-openapi.yml
- filename: cloudera-dfworkload-openapi.yml
  format: yaml
  label: Cloudera DataFlow Workload API
  slug: cloudera-dataflow-workload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-dfworkload-openapi.yml
- filename: cloudera-drscp-openapi.yml
  format: yaml
  label: Cloudera Control Plane Data Recovery API
  slug: cloudera-datarecovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-drscp-openapi.yml
- filename: cloudera-dw-openapi.yml
  format: yaml
  label: Cloudera Data Warehouse API
  slug: cloudera-datawarehouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-dw-openapi.yml
- filename: cloudera-environments-openapi.yml
  format: yaml
  label: Cloudera Environments API
  slug: cloudera-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-environments-openapi.yml
- filename: cloudera-iam-openapi.yml
  format: yaml
  label: Cloudera IAM API
  slug: cloudera-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-iam-openapi.yml
- filename: cloudera-imagecatalog-openapi.yml
  format: yaml
  label: Cloudera Image Catalog API
  slug: cloudera-imagecatalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-imagecatalog-openapi.yml
- filename: cloudera-lakehouseopt-openapi.yml
  format: yaml
  label: Cloudera Lakehouse Optimizer API
  slug: cloudera-lakehouse-optimizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-lakehouseopt-openapi.yml
- filename: cloudera-ml-openapi.yml
  format: yaml
  label: Cloudera AI API
  slug: cloudera-ml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-ml-openapi.yml
- filename: cloudera-opdb-openapi.yml
  format: yaml
  label: Cloudera Operational Database API
  slug: cloudera-operational-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-opdb-openapi.yml
- filename: cloudera-replicationmanager-openapi.yml
  format: yaml
  label: Cloudera Replication Manager API
  slug: cloudera-replicationmanager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-replicationmanager-openapi.yml
auth_types:
- signature
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cloudera Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudera secures its APIs with signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cloudera
provider_slug: cloudera
scheme_count: 1
schemes:
- algorithms:
  - rsav1
  - ed25519v1
  credentials:
    docs: https://docs.cloudera.com/cdp-public-cloud/cloud/api/topics/mc-api-overview.html
    issued_by: Cloudera Management Console (console.cdp.cloudera.com) — a user account must generate an API access key pair before any API call is possible.
    kind: api-access-key-pair
    parts:
    - access key ID
    - private key
  description: Every request to the CDP control plane must be signed. The client builds a canonical request string of httpMethod\ncontentType\ntimestamp\npath\nauthMethod, signs it with the private half of a CDP API access key pair, and sends the signature in x-altus-auth with the matching RFC 1123 timestamp in x-altus-date. Control plane requests are always POST with Content-Type application/json.
  in: header
  name: altusRequestSigning
  parameters:
  - x-altus-auth
  - x-altus-date
  sources:
  - https://github.com/cloudera/cdp-dev-docs/blob/master/api-docs/swagger/request_signing.md
  spec: https://github.com/cloudera/cdp-dev-docs/blob/master/api-docs/swagger/request_signing.md
  tooling:
  - description: Cloudera's own signing helper, shipped inside cdpcurl. The API overview names it as the supported way to generate x-altus-auth / x-altus-date for any HTTP client that is not the CDP CLI or SDK.
    name: cdpv1sign
    package: cdpcurl
    url: https://github.com/cloudera/cdpcurl
  type: signature
slug: cloudera-authentication
source_filename: cloudera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://docs.cloudera.com/cdp-public-cloud/cloud/api/topics/mc-api-overview.html\n  and https://github.com/cloudera/cdp-dev-docs/blob/master/api-docs/swagger/request_signing.md\n  (CDP API Request Signing Specification V1), corroborated by live probes of\n  https://api.us-west-1.cdp.cloudera.com\nsummary:\n  types:\n    - signature\n  api_key_in:\n    - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nnote: >-\n  THE PUBLISHED SWAGGER CARRIES NO securityDefinitions. All 19 CDP control plane\n  service definitions omit the block entirely, so a spec-only derivation produces\n  nothing — the auth model here is documented in prose and in a separate signing\n  specification, not in the contract. That is a real gap worth reporting to\n  Cloudera: a client generated straight from these definitions will not sign its\n  requests and will receive 401 AUTHENTICATION_FAILURE on every call.\nschemes:\n  - name:\
  \ altusRequestSigning\n    type: signature\n    in: header\n    parameters:\n      - x-altus-auth\n      - x-altus-date\n    spec: https://github.com/cloudera/cdp-dev-docs/blob/master/api-docs/swagger/request_signing.md\n    algorithms:\n      - rsav1\n      - ed25519v1\n    description: >-\n      Every request to the CDP control plane must be signed. The client builds a\n      canonical request string of httpMethod\\ncontentType\\ntimestamp\\npath\\nauthMethod,\n      signs it with the private half of a CDP API access key pair, and sends the\n      signature in x-altus-auth with the matching RFC 1123 timestamp in\n      x-altus-date. Control plane requests are always POST with Content-Type\n      application/json.\n    credentials:\n      kind: api-access-key-pair\n      parts:\n        - access key ID\n        - private key\n      issued_by: >-\n        Cloudera Management Console (console.cdp.cloudera.com) — a user account\n        must generate an API access key pair before any API\
  \ call is possible.\n      docs: https://docs.cloudera.com/cdp-public-cloud/cloud/api/topics/mc-api-overview.html\n    tooling:\n      - name: cdpv1sign\n        package: cdpcurl\n        description: >-\n          Cloudera's own signing helper, shipped inside cdpcurl. The API overview\n          names it as the supported way to generate x-altus-auth / x-altus-date\n          for any HTTP client that is not the CDP CLI or SDK.\n        url: https://github.com/cloudera/cdpcurl\n    sources:\n      - https://github.com/cloudera/cdp-dev-docs/blob/master/api-docs/swagger/request_signing.md\nprobes:\n  - url: https://api.us-west-1.cdp.cloudera.com/api/v1/iam/listUsers\n    method: POST\n    sent: no auth headers\n    status: 401\n    body: >-\n      {\"code\":\"AUTHENTICATION_FAILURE\",\"message\":\"No authentication methods used.\n      You must use an authentication method.\"}\n  - url: https://api.us-west-1.cdp.cloudera.com/api/v1/iam/listUsers\n    method: POST\n    sent: x-altus-auth +\
  \ malformed x-altus-date\n    status: 401\n    body: >-\n      {\"code\":\"AUTHENTICATION_FAILURE\",\"message\":\"Cannot parse date time string\n      Fri, 5 Sep 2026 12:00:00 GMT\"}\n    observation: >-\n      The gateway validates the timestamp format before the signature, and the\n      error text names the failing component — useful, specific feedback for an\n      agent building a signed request.\nauthorization:\n  model: rbac\n  note: >-\n    Authorization is separate from authentication and is managed by the CDP IAM\n    service (openapi/cloudera-iam-openapi.yml, 79 operations) — roles, resource\n    roles, groups, machine users and CRN-scoped resource assignments. There are no\n    OAuth scopes: the API is signed with a key pair and the caller's permissions\n    come from the IAM role assignments attached to that user or machine user, so\n    no scopes/ artifact is produced for this provider.\n  operations:\n    - assignUserRole\n    - unassignUserRole\n    - assignUserResourceRole\n\
  \    - unassignUserResourceRole\n    - assignMachineUserRole\n    - assignGroupRole\n    - listRoles\n    - listResourceRoles\n    - listUserAssignedRoles\n    - createMachineUser\n    - createMachineUserAccessKey\nadjacent_surfaces:\n  - name: Cloudera Manager API\n    auth: HTTP basic auth with Cloudera Manager UI credentials; a session cookie may be reused on subsequent requests.\n    docs: https://cloudera.github.io/cm_api/\n  - name: Cloudera AI (CML) workbench API v2\n    auth: API key issued from the workbench, passed to the cmlapi SDK.\n  - name: NiFi via Apache Knox\n    auth: Knox bearer token, cookie or passcode token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/authentication/cloudera-authentication.yml
summary_line: signature · 1 scheme
tags:
- Big Data
- Data Engineering
- Data Lakehouse
- Data Platform
- Data Warehouse
- Hadoop
- Hybrid Cloud
- Machine-Learning
- Streaming
---
