---
api_key_in:
- header
api_specs:
- filename: imperva-account-management-api-openapi.yml
  format: yaml
  label: Imperva Account Management API
  slug: imperva-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/openapi/imperva-account-management-api-openapi.yml
- filename: imperva-administration-api-openapi.yml
  format: yaml
  label: Imperva Administration API
  slug: imperva-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/openapi/imperva-administration-api-openapi.yml
- filename: imperva-auth-api-openapi.yml
  format: yaml
  label: Imperva Auth API
  slug: imperva-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/openapi/imperva-auth-api-openapi.yml
- filename: imperva-conf-api-openapi.yml
  format: yaml
  label: Imperva Conf API
  slug: imperva-conf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/openapi/imperva-conf-api-openapi.yml
- filename: imperva-ddos-for-networks-test-alerts-api-openapi.yml
  format: yaml
  label: Imperva DDoS for Networks Test Alerts API
  slug: imperva-ddos-for-networks-test-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/openapi/imperva-ddos-for-networks-test-alerts-api-openapi.yml
- filename: imperva-ddos-protection-for-individual-ips-api-openapi.yml
  format: yaml
  label: Imperva DDoS Protection for Individual IPs API
  slug: imperva-ddos-protection-for-individual-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/openapi/imperva-ddos-protection-for-individual-ips-api-openapi.yml
- filename: imperva-experimental-api-openapi.yml
  format: yaml
  label: Imperva Experimental API
  slug: imperva-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/openapi/imperva-experimental-api-openapi.yml
- filename: imperva-integrations-api-openapi.yml
  format: yaml
  label: Imperva Integrations API
  slug: imperva-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/openapi/imperva-integrations-api-openapi.yml
- filename: imperva-login-protect-api-openapi.yml
  format: yaml
  label: Imperva Login Protect API
  slug: imperva-login-protect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/openapi/imperva-login-protect-api-openapi.yml
- filename: imperva-management-api-openapi.yml
  format: yaml
  label: Imperva Management API
  slug: imperva-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/openapi/imperva-management-api-openapi.yml
- filename: imperva-site-management-api-openapi.yml
  format: yaml
  label: Imperva Site Management API
  slug: imperva-site-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/openapi/imperva-site-management-api-openapi.yml
- filename: imperva-status-api-openapi.yml
  format: yaml
  label: Imperva Status API
  slug: imperva-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/openapi/imperva-status-api-openapi.yml
- filename: imperva-traffic-statistics-and-logs-api-openapi.yml
  format: yaml
  label: Imperva Traffic Statistics and Logs API
  slug: imperva-traffic-statistics-and-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/openapi/imperva-traffic-statistics-and-logs-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Imperva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Imperva secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Imperva
provider_slug: imperva
scheme_count: 3
schemes:
- in: header
  name: api_id
  parameter: x-API-Id
  sources:
  - openapi/imperva-cloud-application-security-openapi.yml
  type: apiKey
- in: header
  name: api_key
  parameter: x-API-Key
  sources:
  - openapi/imperva-cloud-application-security-openapi.yml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/imperva-securesphere-openapi.yml
  type: http
slug: imperva-authentication
source_filename: imperva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/imperva-cloud-application-security-openapi.yml, openapi/imperva-securesphere-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_id\n  type: apiKey\n  in: header\n  parameter: x-API-Id\n  sources:\n  - openapi/imperva-cloud-application-security-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-API-Key\n  sources:\n  - openapi/imperva-cloud-application-security-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/imperva-securesphere-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/authentication/imperva-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Security
- Cybersecurity
- WAF
- DDoS Protection
- API Security
- Bot Management
- Data Security
- Cloud Security
---
