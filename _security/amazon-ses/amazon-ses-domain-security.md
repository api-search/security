---
api_specs:
- filename: amazon-ses-email-api-openapi.yml
  format: yaml
  label: Amazon SES Email API
  slug: amazon-ses-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-email-api-openapi.yml
- filename: amazon-ses-addon-instance-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Addon Instance API
  slug: amazon-ses-addon-instance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-addon-instance-api-openapi.yml
- filename: amazon-ses-addon-subscription-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Addon Subscription API
  slug: amazon-ses-addon-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-addon-subscription-api-openapi.yml
- filename: amazon-ses-address-list-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Address List API
  slug: amazon-ses-address-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-address-list-api-openapi.yml
- filename: amazon-ses-address-list-import-job-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Address List Import Job API
  slug: amazon-ses-address-list-import-job-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-address-list-import-job-api-openapi.yml
- filename: amazon-ses-archive-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Archive API
  slug: amazon-ses-archive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-archive-api-openapi.yml
- filename: amazon-ses-archive-export-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Archive Export API
  slug: amazon-ses-archive-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-archive-export-api-openapi.yml
- filename: amazon-ses-archive-search-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Archive Search API
  slug: amazon-ses-archive-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-archive-search-api-openapi.yml
- filename: amazon-ses-configuration-set-tracking-option-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Configuration Set Tracking Option API
  slug: amazon-ses-configuration-set-tracking-option-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-configuration-set-tracking-option-api-openapi.yml
- filename: amazon-ses-identity-policy-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Identity Policy API
  slug: amazon-ses-identity-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-identity-policy-api-openapi.yml
- filename: amazon-ses-ingress-point-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Ingress Point API
  slug: amazon-ses-ingress-point-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-ingress-point-api-openapi.yml
- filename: amazon-ses-operations-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Operations API
  slug: amazon-ses-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-operations-api-openapi.yml
- filename: amazon-ses-receipt-filter-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Receipt Filter API
  slug: amazon-ses-receipt-filter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-receipt-filter-api-openapi.yml
- filename: amazon-ses-receipt-rule-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Receipt Rule API
  slug: amazon-ses-receipt-rule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-receipt-rule-api-openapi.yml
- filename: amazon-ses-receipt-rule-set-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Receipt Rule Set API
  slug: amazon-ses-receipt-rule-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-receipt-rule-set-api-openapi.yml
- filename: amazon-ses-relay-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Relay API
  slug: amazon-ses-relay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-relay-api-openapi.yml
- filename: amazon-ses-rule-set-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Rule Set API
  slug: amazon-ses-rule-set-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-rule-set-api-openapi.yml
- filename: amazon-ses-template-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Template API
  slug: amazon-ses-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-template-api-openapi.yml
- filename: amazon-ses-traffic-policy-api-openapi.yml
  format: yaml
  label: Amazon SES Ses Traffic Policy API
  slug: amazon-ses-traffic-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-ses/openapi/amazon-ses-traffic-policy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 26 05:01:14 2027 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon SES Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon SES, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon SES
provider_slug: amazon-ses
slug: amazon-ses-domain-security
source_filename: amazon-ses-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 26 05:01:14 2027 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-ses/security/amazon-ses-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Web Services
- Email
- Email Deliverability
- Email Service
- Marketing Email
- Notification
- SMTP
- Transactional Email
- Bulk Email
- Email Receiving
- DKIM
- Messaging
- Cloud Infrastructure
---
