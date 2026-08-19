---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Cloudexmachina Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloud Ex Machina declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cloud Ex Machina
provider_slug: cloudexmachina
scheme_count: 1
schemes:
- details:
    acs_url: https://auth.<tenant_id>.cloudexmachina.io/saml2/idpresponse
    assertion_encryption: unencrypted
    assertion_signed: true
    attribute_statements:
    - given_name
    - last_name
    - email
    audience_uri: urn:amazon:cognito:sp:<cxm_cognito_pool_id>
    authn_context_class_ref: PasswordProtectedTransport
    default_relay_state: https://<tenant_id>.cloudexmachina.io/cloud-explorer
    digest_algorithm: SHA256
    force_authn_honored: true
    name_id_format: Unspecified
    response_signed: true
    signature_algorithm: RSA_SHA256
    signed_request: disabled
    single_logout: disabled
    username_format: email
  federation_broker: Amazon Cognito
  idp_documented: Okta
  name: saml-sso
  provisioning:
    note: SSO is not self-service. The setup guide instructs the customer to "share the Metadata URL with CxM on Slack or email. We will enable the SSO for you as fast as we can." Cloud ex Machina must also hand the customer the internal cxm_cognito_pool_id before the IdP app can be configured, so onboarding is a human, vendor-mediated step.
    self_service: false
  source: https://docs.cloudexmachina.io/setup/sso/okta
  type: saml2
slug: cloudexmachina-authentication
source_filename: cloudexmachina-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nsource: https://docs.cloudexmachina.io/setup/sso/okta\nscope: platform-sso\napi_authentication: none\nnote: >-\n  IMPORTANT SCOPE NOTE — read before using this artifact. Cloud ex Machina publishes NO public API,\n  so there is no API authentication scheme to document: no OpenAPI securitySchemes, no API keys, no\n  bearer tokens, no OAuth authorization server, no personal access tokens. derive-authentication.py\n  was not run because there is no OpenAPI in this repo to derive from. What this artifact records is\n  the authentication Cloud ex Machina DOES publish and document: how a human operator authenticates\n  into their per-tenant web application. The API keys that appear in Cloud ex Machina's integration\n  docs are THIRD-PARTY credentials (Anthropic, GitLab, ServiceNow) that a customer supplies TO Cloud\n  ex Machina so it can call those vendors — they are not credentials Cloud ex Machina issues.\ntenancy:\n  model: per-tenant\
  \ subdomain\n  app_url_pattern: https://<tenant_id>.cloudexmachina.io\n  auth_url_pattern: https://auth.<tenant_id>.cloudexmachina.io\n  shared_app_host: https://app.cloudexmachina.io\nschemes:\n- name: saml-sso\n  type: saml2\n  idp_documented: Okta\n  federation_broker: Amazon Cognito\n  source: https://docs.cloudexmachina.io/setup/sso/okta\n  details:\n    acs_url: https://auth.<tenant_id>.cloudexmachina.io/saml2/idpresponse\n    audience_uri: 'urn:amazon:cognito:sp:<cxm_cognito_pool_id>'\n    default_relay_state: https://<tenant_id>.cloudexmachina.io/cloud-explorer\n    name_id_format: Unspecified\n    response_signed: true\n    assertion_signed: true\n    assertion_encryption: unencrypted\n    signature_algorithm: RSA_SHA256\n    digest_algorithm: SHA256\n    single_logout: disabled\n    signed_request: disabled\n    authn_context_class_ref: PasswordProtectedTransport\n    force_authn_honored: true\n    username_format: email\n    attribute_statements: [given_name, last_name, email]\n\
  \  provisioning:\n    self_service: false\n    note: >-\n      SSO is not self-service. The setup guide instructs the customer to \"share the Metadata URL\n      with CxM on Slack or email. We will enable the SSO for you as fast as we can.\" Cloud ex\n      Machina must also hand the customer the internal cxm_cognito_pool_id before the IdP app can\n      be configured, so onboarding is a human, vendor-mediated step.\ncloud_access:\n  model: read-only, agentless cross-account role assumption\n  aws:\n    mechanism: cross-account IAM role\n    provisioned_by:\n    - terraform module cxmlabs/cxm-integration/aws\n    - cloudformation template cxmlabs/cloudformation-aws-cxm-integration\n    source: https://docs.cloudexmachina.io/setup/csp-configuration/aws-setup\n  azure:\n    source: https://docs.cloudexmachina.io/setup/csp-configuration/azure-setup/overview\n  gcp:\n    source: https://docs.cloudexmachina.io/setup/csp-configuration/gcp-setup\n  kubernetes:\n    source: https://docs.cloudexmachina.io/setup/csp-configuration/k8s-setup\n\
  outbound_credentials_collected:\n  note: >-\n    Credentials the customer gives Cloud ex Machina for third-party systems. Listed for\n    completeness — these belong to the named vendor, not to Cloud ex Machina.\n  entries:\n  - {provider: Anthropic, mechanism: analytics API key + API version header (default 2023-06-01)}\n  - {provider: Anthropic, mechanism: Administrator API key}\n  - {provider: ServiceNow, mechanism: OAuth 2.0 client credentials}\n  - {provider: GitHub, mechanism: OAuth app connect flow}\n  - {provider: GitLab, mechanism: OAuth connect flow + API base URL for self-hosted}\n  - {provider: Slack / Microsoft Teams, mechanism: OAuth connect flow}\n  - {provider: Jira / Linear / Notion, mechanism: OAuth connect flow}\n  integration_broker: Nango (named as a subprocessor for \"Product integrations\")\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudexmachina/refs/heads/main/authentication/cloudexmachina-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Infrastructure
- Cloud
- FinOps
- Cloud Cost Optimization
- Cloud Governance
- AI Agents
- Cloud Management
- Terraform
- Kubernetes
---
