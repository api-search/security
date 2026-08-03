---
api_key_in: []
api_specs:
- filename: pingcap-tidb-cloud-starter-essential-v1beta1-openapi-original.json
  format: json
  label: TiDB Cloud Starter and Essential API (v1beta1)
  slug: tidb-cloud-starter-and-essential-api-v1beta1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-starter-essential-v1beta1-openapi-original.json
- filename: pingcap-tidb-cloud-dedicated-v1beta1-openapi-original.json
  format: json
  label: TiDB Cloud Dedicated API (v1beta1)
  slug: tidb-cloud-dedicated-api-v1beta1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-dedicated-v1beta1-openapi-original.json
- filename: pingcap-tidb-cloud-iam-v1beta1-openapi-original.json
  format: json
  label: TiDB Cloud IAM API (v1beta1)
  slug: tidb-cloud-iam-api-v1beta1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-iam-v1beta1-openapi-original.json
- filename: pingcap-tidb-cloud-billing-v1beta1-openapi-original.json
  format: json
  label: TiDB Cloud Billing API (v1beta1)
  slug: tidb-cloud-billing-api-v1beta1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-billing-v1beta1-openapi-original.json
- filename: pingcap-tidb-cloud-data-service-v1beta1-openapi-original.json
  format: json
  label: TiDB Cloud Data Service API (v1beta1)
  slug: tidb-cloud-data-service-api-v1beta1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-data-service-v1beta1-openapi-original.json
- filename: pingcap-tidb-cloud-v1beta-openapi-original.json
  format: json
  label: TiDB Cloud API (v1beta, legacy)
  slug: tidb-cloud-api-v1beta-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-v1beta-openapi-original.json
- filename: pingcap-tidb-cloud-zero-v1alpha1-openapi-original.json
  format: json
  label: TiDB Cloud Zero API (v1alpha1)
  slug: tidb-cloud-zero-api-v1alpha1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-cloud-zero-v1alpha1-openapi-original.json
- filename: pingcap-tidb-dm-openapi-original.yaml
  format: yaml
  label: TiDB Data Migration (DM) OpenAPI
  slug: tidb-data-migration-dm-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-tidb-dm-openapi-original.yaml
- filename: pingcap-ossinsight-public-api-openapi-original.yaml
  format: yaml
  label: OSS Insight Public API
  slug: oss-insight-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/openapi/pingcap-ossinsight-public-api-openapi-original.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Pingcap Authentication
name_suffix: Authentication
oauth_flows: []
overview: PingCAP secures its APIs with http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PingCAP
provider_slug: pingcap
scheme_count: 4
schemes:
- applies_to:
  - api.tidbcloud.com
  - serverless.tidbapi.com
  - dedicated.tidbapi.com
  - iam.tidbapi.com
  - billing.tidbapi.com
  - dataservice.tidbapi.com
  credential:
    kind: key pair
    private_key: password component; displayed only once at creation and never retrievable again
    public_key: username component; visible in the console
  description: Every TiDB Cloud API request is authenticated with HTTP Digest Authentication. The API key public key acts as the username and the private key acts as the password, so the private key is never transmitted over the network. Missing or invalid credentials return 401.
  example: curl --digest --user 'YOUR_PUBLIC_KEY:YOUR_PRIVATE_KEY' --request GET --url https://serverless.tidbapi.com/v1beta1/clusters
  managed_via:
  - https://tidbcloud.com/org-settings/api-keys
  - openapi/pingcap-tidb-cloud-iam-v1beta1-openapi-original.json (/apikeys CRUD)
  name: TiDB Cloud organization API key
  rfc: RFC 7616 (HTTP Digest Access Authentication)
  scheme: digest
  scope: Organization-wide. The key carries a role (for example org:owner) and an optional project scope, configured at creation time in Organization Settings > API Keys.
  sources:
  - pingcap-ossinsight-public-api-openapi-original.yaml
  - pingcap-tidb-cloud-billing-v1beta1-openapi-original.json
  - pingcap-tidb-cloud-data-service-v1beta1-openapi-original.json
  - pingcap-tidb-cloud-dedicated-v1beta1-openapi-original.json
  - pingcap-tidb-cloud-iam-v1beta1-openapi-original.json
  - pingcap-tidb-cloud-starter-essential-v1beta1-openapi-original.json
  - pingcap-tidb-cloud-v1beta-openapi-original.json
  - pingcap-tidb-cloud-zero-v1alpha1-openapi-original.json
  - pingcap-tidb-dm-openapi-original.yaml
  type: http
- description: A separate key class used to call deployed Data Service endpoints (reading data in a cluster), distinct from the organization API key used to manage Data Apps and platform resources.
  docs: https://docs.pingcap.com/tidbcloud/api/v1beta1/dataservice/
  name: TiDB Cloud Data Service Data API key
  scheme: digest
  sources:
  - openapi/pingcap-tidb-cloud-data-service-v1beta1-openapi-original.json
  type: http
- description: The TiDB Cloud Zero provisioning endpoint is deliberately unauthenticated and free to call; it returns a short-lived MySQL-compatible instance with generated credentials that expires in 30 days unless claimed.
  name: No authentication (TiDB Cloud Zero)
  sources:
  - openapi/pingcap-tidb-cloud-zero-v1alpha1-openapi-original.json
  type: none
- description: The OSS Insight public analytics API is read-only and open; no credential is documented.
  name: No authentication (OSS Insight Public API)
  sources:
  - openapi/pingcap-ossinsight-public-api-openapi-original.yaml
  type: none
slug: pingcap-authentication
source_filename: pingcap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://docs.pingcap.com/tidbcloud/api-overview/\ndocs: https://docs.pingcap.com/tidbcloud/api/v1beta#section/Authentication\nnote: None of the published TiDB Cloud OpenAPI/Swagger documents declare a securityDefinitions block; the authentication\n  contract is documented only in prose in the API overview and in each spec's info.description. This profile is\n  searched from those docs, not derived from the specs.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - digest\n  api_key_in: []\n  oauth2_flows: []\n  spec_declared: false\nschemes:\n- name: TiDB Cloud organization API key\n  type: http\n  scheme: digest\n  rfc: RFC 7616 (HTTP Digest Access Authentication)\n  description: Every TiDB Cloud API request is authenticated with HTTP Digest Authentication. The API key public\n    key acts as the username and the private key acts as the password, so the private key is never transmitted over\n    the network. Missing or invalid\
  \ credentials return 401.\n  credential:\n    kind: key pair\n    public_key: username component; visible in the console\n    private_key: password component; displayed only once at creation and never retrievable again\n  scope: Organization-wide. The key carries a role (for example org:owner) and an optional project scope, configured\n    at creation time in Organization Settings > API Keys.\n  managed_via:\n  - https://tidbcloud.com/org-settings/api-keys\n  - openapi/pingcap-tidb-cloud-iam-v1beta1-openapi-original.json (/apikeys CRUD)\n  example: curl --digest --user 'YOUR_PUBLIC_KEY:YOUR_PRIVATE_KEY' --request GET --url https://serverless.tidbapi.com/v1beta1/clusters\n  applies_to:\n  - api.tidbcloud.com\n  - serverless.tidbapi.com\n  - dedicated.tidbapi.com\n  - iam.tidbapi.com\n  - billing.tidbapi.com\n  - dataservice.tidbapi.com\n  sources:\n  - pingcap-ossinsight-public-api-openapi-original.yaml\n  - pingcap-tidb-cloud-billing-v1beta1-openapi-original.json\n  - pingcap-tidb-cloud-data-service-v1beta1-openapi-original.json\n\
  \  - pingcap-tidb-cloud-dedicated-v1beta1-openapi-original.json\n  - pingcap-tidb-cloud-iam-v1beta1-openapi-original.json\n  - pingcap-tidb-cloud-starter-essential-v1beta1-openapi-original.json\n  - pingcap-tidb-cloud-v1beta-openapi-original.json\n  - pingcap-tidb-cloud-zero-v1alpha1-openapi-original.json\n  - pingcap-tidb-dm-openapi-original.yaml\n- name: TiDB Cloud Data Service Data API key\n  type: http\n  scheme: digest\n  description: A separate key class used to call deployed Data Service endpoints (reading data in a cluster), distinct\n    from the organization API key used to manage Data Apps and platform resources.\n  docs: https://docs.pingcap.com/tidbcloud/api/v1beta1/dataservice/\n  sources:\n  - openapi/pingcap-tidb-cloud-data-service-v1beta1-openapi-original.json\n- name: No authentication (TiDB Cloud Zero)\n  type: none\n  description: The TiDB Cloud Zero provisioning endpoint is deliberately unauthenticated and free to call; it returns\n    a short-lived MySQL-compatible\
  \ instance with generated credentials that expires in 30 days unless claimed.\n  sources:\n  - openapi/pingcap-tidb-cloud-zero-v1alpha1-openapi-original.json\n- name: No authentication (OSS Insight Public API)\n  type: none\n  description: The OSS Insight public analytics API is read-only and open; no credential is documented.\n  sources:\n  - openapi/pingcap-ossinsight-public-api-openapi-original.yaml\ndatabase_auth:\n  note: Data-plane access to a TiDB cluster is MySQL protocol authentication (SQL user + password) over TLS, managed\n    with ticloud serverless sql-user or in the console. TiDB Cloud console sign-in additionally supports OAuth 2.0\n    / SSO, but the management API itself does not accept OAuth tokens.\n  docs: https://docs.pingcap.com/tidbcloud/tidb-cloud-quickstart/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pingcap/refs/heads/main/authentication/pingcap-authentication.yml
summary_line: http · 4 schemes
tags:
- distributed-sql
- database
- tidb
- htap
- mysql-compatible
- cloud-database
- dbaas
- vector-search
- data-migration
- change-data-capture
- open-source
- infrastructure
---
