---
api_specs:
- filename: amazon-billing-and-cost-management-anomaly-detection-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Anomaly Detection API
  slug: amazon-billing-and-cost-management-anomaly-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-anomaly-detection-api-openapi.yml
- filename: amazon-billing-and-cost-management-budget-actions-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Budget Actions API
  slug: amazon-billing-and-cost-management-budget-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-budget-actions-api-openapi.yml
- filename: amazon-billing-and-cost-management-budgets-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Budgets API
  slug: amazon-billing-and-cost-management-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-budgets-api-openapi.yml
- filename: amazon-billing-and-cost-management-cost-and-usage-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Cost And Usage API
  slug: amazon-billing-and-cost-management-cost-and-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-cost-and-usage-api-openapi.yml
- filename: amazon-billing-and-cost-management-cost-categories-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Cost Categories API
  slug: amazon-billing-and-cost-management-cost-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-cost-categories-api-openapi.yml
- filename: amazon-billing-and-cost-management-forecasting-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Forecasting API
  slug: amazon-billing-and-cost-management-forecasting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-forecasting-api-openapi.yml
- filename: amazon-billing-and-cost-management-notifications-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Notifications API
  slug: amazon-billing-and-cost-management-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-notifications-api-openapi.yml
- filename: amazon-billing-and-cost-management-recommendations-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Recommendations API
  slug: amazon-billing-and-cost-management-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-recommendations-api-openapi.yml
- filename: amazon-billing-and-cost-management-tags-api-openapi.yml
  format: yaml
  label: Amazon Billing And Cost Management Tags API
  slug: amazon-billing-and-cost-management-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/openapi/amazon-billing-and-cost-management-tags-api-openapi.yml
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
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: ce.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Billing And Cost Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Billing And Cost Management, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Billing And Cost Management
provider_slug: amazon-billing-and-cost-management
slug: amazon-billing-and-cost-management-domain-security
source_filename: amazon-billing-and-cost-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: ce.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-billing-and-cost-management/refs/heads/main/security/amazon-billing-and-cost-management-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Cost Management
- Cost Explorer
- Budgets
- Cost Optimization
- FinOps
- Amazon Web Services
---
