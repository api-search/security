---
api_specs:
- filename: microsoft-azure-policy-policyassignments-api-openapi.yml
  format: yaml
  label: Azure Policy Policy Assignments API
  slug: microsoft-azure-policy-policyassignments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-policy/openapi/microsoft-azure-policy-policyassignments-api-openapi.yml
- filename: microsoft-azure-policy-policydefinitions-api-openapi.yml
  format: yaml
  label: Azure Policy Policy Definitions API
  slug: microsoft-azure-policy-policydefinitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-policy/openapi/microsoft-azure-policy-policydefinitions-api-openapi.yml
- filename: microsoft-azure-policy-policydefinitionversions-api-openapi.yml
  format: yaml
  label: Azure Policy Policy Definition Versions API
  slug: microsoft-azure-policy-policydefinitionversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-policy/openapi/microsoft-azure-policy-policydefinitionversions-api-openapi.yml
- filename: microsoft-azure-policy-policysetdefinitions-api-openapi.yml
  format: yaml
  label: Azure Policy Policy Set Definitions API
  slug: microsoft-azure-policy-policysetdefinitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-policy/openapi/microsoft-azure-policy-policysetdefinitions-api-openapi.yml
- filename: microsoft-azure-policy-policysetdefinitionversions-api-openapi.yml
  format: yaml
  label: Azure Policy Policy Set Definition Versions API
  slug: microsoft-azure-policy-policysetdefinitionversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-policy/openapi/microsoft-azure-policy-policysetdefinitionversions-api-openapi.yml
- filename: microsoft-azure-policy-providers-api-openapi.yml
  format: yaml
  label: Azure Policy Providers API
  slug: microsoft-azure-policy-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-policy/openapi/microsoft-azure-policy-providers-api-openapi.yml
- filename: microsoft-azure-policy-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Policy Subscriptions API
  slug: microsoft-azure-policy-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-policy/openapi/microsoft-azure-policy-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 19:05:38 2027 GMT
  host: azure.microsoft.com
  hsts: null
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
name: Azure Policy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Policy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Policy
provider_slug: microsoft-azure-policy
slug: microsoft-azure-policy-domain-security
source_filename: microsoft-azure-policy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 19:05:38 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-policy/security/microsoft-azure-policy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- Governance
- Policy
- Resource Management
---
