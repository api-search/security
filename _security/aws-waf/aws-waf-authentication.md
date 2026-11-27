---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: aws-waf-aws-wafv2-api-api-openapi.yml
  format: yaml
  label: AWS WAF AWS WAFV2 API
  slug: aws-waf-aws-wafv2-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-aws-wafv2-api-api-openapi.yml
- filename: aws-waf-ip-sets-api-openapi.yml
  format: yaml
  label: AWS WAF IP Sets API
  slug: aws-waf-ip-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-ip-sets-api-openapi.yml
- filename: aws-waf-rule-groups-api-openapi.yml
  format: yaml
  label: AWS WAF Rule Groups API
  slug: aws-waf-rule-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-rule-groups-api-openapi.yml
- filename: aws-waf-web-acls-api-openapi.yml
  format: yaml
  label: AWS WAF Web ACLs API
  slug: aws-waf-web-acls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-web-acls-api-openapi.yml
- filename: aws-waf-byte-match-set-api-openapi.yml
  format: yaml
  label: AWS WAF Waf Byte Match Set API
  slug: aws-waf-byte-match-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-byte-match-set-api-openapi.yml
- filename: aws-waf-geo-match-set-api-openapi.yml
  format: yaml
  label: AWS WAF Waf Geo Match Set API
  slug: aws-waf-geo-match-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-geo-match-set-api-openapi.yml
- filename: aws-waf-logging-configuration-api-openapi.yml
  format: yaml
  label: AWS WAF Waf Logging Configuration API
  slug: aws-waf-logging-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-logging-configuration-api-openapi.yml
- filename: aws-waf-permission-policy-api-openapi.yml
  format: yaml
  label: AWS WAF Waf Permission Policy API
  slug: aws-waf-permission-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-permission-policy-api-openapi.yml
- filename: aws-waf-rate-based-rule-api-openapi.yml
  format: yaml
  label: AWS WAF Waf Rate Based Rule API
  slug: aws-waf-rate-based-rule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-rate-based-rule-api-openapi.yml
- filename: aws-waf-regex-match-set-api-openapi.yml
  format: yaml
  label: AWS WAF Waf Regex Match Set API
  slug: aws-waf-regex-match-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-regex-match-set-api-openapi.yml
- filename: aws-waf-regex-pattern-set-api-openapi.yml
  format: yaml
  label: AWS WAF Waf Regex Pattern Set API
  slug: aws-waf-regex-pattern-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-regex-pattern-set-api-openapi.yml
- filename: aws-waf-rule-api-openapi.yml
  format: yaml
  label: AWS WAF Waf Rule API
  slug: aws-waf-rule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-rule-api-openapi.yml
- filename: aws-waf-size-constraint-set-api-openapi.yml
  format: yaml
  label: AWS WAF Waf Size Constraint Set API
  slug: aws-waf-size-constraint-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-size-constraint-set-api-openapi.yml
- filename: aws-waf-sql-injection-match-set-api-openapi.yml
  format: yaml
  label: AWS WAF Waf Sql Injection Match Set API
  slug: aws-waf-sql-injection-match-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-sql-injection-match-set-api-openapi.yml
- filename: aws-waf-xss-match-set-api-openapi.yml
  format: yaml
  label: AWS WAF Waf Xss Match Set API
  slug: aws-waf-xss-match-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-xss-match-set-api-openapi.yml
- filename: aws-waf-api-key-api-openapi.yml
  format: yaml
  label: AWS WAF Waf Api Key API
  slug: aws-waf-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-api-key-api-openapi.yml
- filename: aws-waf-operations-api-openapi.yml
  format: yaml
  label: AWS WAF Waf Operations API
  slug: aws-waf-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aws-waf/openapi/aws-waf-operations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AWS WAF Authentication
name_suffix: Authentication
oauth_flows: []
overview: AWS WAF secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AWS WAF
provider_slug: aws-waf
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/aws-waf-api-key-api-openapi.yml
  - openapi/aws-waf-aws-wafv2-api-api-openapi.yml
  - openapi/aws-waf-byte-match-set-api-openapi.yml
  - openapi/aws-waf-geo-match-set-api-openapi.yml
  - openapi/aws-waf-ip-sets-api-openapi.yml
  - openapi/aws-waf-logging-configuration-api-openapi.yml
  - openapi/aws-waf-operations-api-openapi.yml
  - openapi/aws-waf-permission-policy-api-openapi.yml
  - openapi/aws-waf-rate-based-rule-api-openapi.yml
  - openapi/aws-waf-regex-match-set-api-openapi.yml
  - openapi/aws-waf-regex-pattern-set-api-openapi.yml
  - openapi/aws-waf-rule-api-openapi.yml
  - openapi/aws-waf-rule-groups-api-openapi.yml
  - openapi/aws-waf-size-constraint-set-api-openapi.yml
  - openapi/aws-waf-sql-injection-match-set-api-openapi.yml
  - openapi/aws-waf-web-acls-api-openapi.yml
  - openapi/aws-waf-xss-match-set-api-openapi.yml
  type: apiKey
slug: aws-waf-authentication
source_filename: aws-waf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/aws-waf-api-key-api-openapi.yml, openapi/aws-waf-aws-wafv2-api-api-openapi.yml,\n  openapi/aws-waf-byte-match-set-api-openapi.yml, openapi/aws-waf-geo-match-set-api-openapi.yml,\n  openapi/aws-waf-ip-sets-api-openapi.yml, openapi/aws-waf-logging-configuration-api-openapi.yml,\n  openapi/aws-waf-operations-api-openapi.yml, openapi/aws-waf-permission-policy-api-openapi.yml,\n  openapi/aws-waf-rate-based-rule-api-openapi.yml, openapi/aws-waf-regex-match-set-api-openapi.yml,\n  openapi/aws-waf-regex-pattern-set-api-openapi.yml, openapi/aws-waf-rule-api-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials). Not a\
  \ bearer token.\n  sources:\n  - openapi/aws-waf-api-key-api-openapi.yml\n  - openapi/aws-waf-aws-wafv2-api-api-openapi.yml\n  - openapi/aws-waf-byte-match-set-api-openapi.yml\n  - openapi/aws-waf-geo-match-set-api-openapi.yml\n  - openapi/aws-waf-ip-sets-api-openapi.yml\n  - openapi/aws-waf-logging-configuration-api-openapi.yml\n  - openapi/aws-waf-operations-api-openapi.yml\n  - openapi/aws-waf-permission-policy-api-openapi.yml\n  - openapi/aws-waf-rate-based-rule-api-openapi.yml\n  - openapi/aws-waf-regex-match-set-api-openapi.yml\n  - openapi/aws-waf-regex-pattern-set-api-openapi.yml\n  - openapi/aws-waf-rule-api-openapi.yml\n  - openapi/aws-waf-rule-groups-api-openapi.yml\n  - openapi/aws-waf-size-constraint-set-api-openapi.yml\n  - openapi/aws-waf-sql-injection-match-set-api-openapi.yml\n  - openapi/aws-waf-web-acls-api-openapi.yml\n  - openapi/aws-waf-xss-match-set-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/aws-waf/authentication/aws-waf-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Web Application Firewall
- DDoS Protection
- Bot Management
- Edge Security
- Cloud
- Amazon Web Services
---
