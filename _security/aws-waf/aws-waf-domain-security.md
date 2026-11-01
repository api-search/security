---
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
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: wafv2.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aws Waf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AWS WAF, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AWS WAF
provider_slug: aws-waf
slug: aws-waf-domain-security
source_filename: aws-waf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: wafv2.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/aws-waf/security/aws-waf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Web Application Firewall
- DDoS Protection
- Bot Management
- Edge Security
- Cloud
---
