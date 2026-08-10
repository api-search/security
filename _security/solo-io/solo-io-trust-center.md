---
api_specs:
- filename: solo-io-api-keys-api-openapi.yml
  format: yaml
  label: Solo.io API Keys API
  slug: solo-io-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-api-keys-api-openapi.yml
- filename: solo-io-api-products-api-openapi.yml
  format: yaml
  label: Solo.io API Products API
  slug: solo-io-api-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-api-products-api-openapi.yml
- filename: solo-io-apis-api-openapi.yml
  format: yaml
  label: Solo.io AP Is API
  slug: solo-io-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-apis-api-openapi.yml
- filename: solo-io-applications-api-openapi.yml
  format: yaml
  label: Solo.io Applications API
  slug: solo-io-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-applications-api-openapi.yml
- filename: solo-io-apps-api-openapi.yml
  format: yaml
  label: Solo.io Apps API
  slug: solo-io-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-apps-api-openapi.yml
- filename: solo-io-auth-api-openapi.yml
  format: yaml
  label: Solo.io Auth API
  slug: solo-io-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-auth-api-openapi.yml
- filename: solo-io-health-api-openapi.yml
  format: yaml
  label: Solo.io Health API
  slug: solo-io-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-health-api-openapi.yml
- filename: solo-io-me-api-openapi.yml
  format: yaml
  label: Solo.io Me API
  slug: solo-io-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-me-api-openapi.yml
- filename: solo-io-metadata-api-openapi.yml
  format: yaml
  label: Solo.io Metadata API
  slug: solo-io-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-metadata-api-openapi.yml
- filename: solo-io-oauth-credentials-api-openapi.yml
  format: yaml
  label: Solo.io OAUTH Credentials API
  slug: solo-io-oauth-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-oauth-credentials-api-openapi.yml
- filename: solo-io-subscriptions-api-openapi.yml
  format: yaml
  label: Solo.io Subscriptions API
  slug: solo-io-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-subscriptions-api-openapi.yml
- filename: solo-io-teams-api-openapi.yml
  format: yaml
  label: Solo.io Teams API
  slug: solo-io-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-teams-api-openapi.yml
- filename: solo-io-user-api-openapi.yml
  format: yaml
  label: Solo.io User API
  slug: solo-io-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-user-api-openapi.yml
- filename: solo-io-users-api-openapi.yml
  format: yaml
  label: Solo.io Users API
  slug: solo-io-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-users-api-openapi.yml
- filename: solo-io-webhooks-api-openapi.yml
  format: yaml
  label: Solo.io Webhooks API
  slug: solo-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-webhooks-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Solo Io Trust Center
name_suffix: Trust Center
overview: Solo.io maintains a public trust center covering its security and compliance posture.
provider_name: Solo.io
provider_slug: solo-io
slug: solo-io-trust-center
source_filename: solo-io-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nprobe: true\nurl: https://trust.solo.io/\ntitle: Solo Trust Center\nplatform: Vanta\ncertifications: []\ncertifications_note: >-\n  The trust center resolves (HTTP 200) and is titled \"Solo Trust Center\", but it is a\n  Vanta-hosted single-page application: every path under trust.solo.io — including\n  /resources and /documents — returns the identical 4.5 KB HTML shell to a client that does\n  not execute JavaScript. No certification names could be read without rendering, and no\n  SOC 2 / ISO 27001 / PCI DSS / HIPAA / FedRAMP claim appears on any statically fetchable\n  Solo.io page. The list above is left EMPTY rather than populated by inference.\ndescription_from_page: >-\n  \"Solo.io is a cloud-native software company founded in 2017 delivering API gateway,\n  service mesh, and agentic AI connectivity products — including Solo Enterprise for Istio,\n  kgateway, agentgateway, and kagent — built on the open-source Envoy and Istio\
  \ projects.\"\nx-evidence:\n- {source: 'https://trust.solo.io/', http_status: 200, content_type: text/html, bytes: 4477,\n   detected: Vanta trust report shell}\n- {source: 'https://trust.solo.io/resources', http_status: 200, note: SPA catch-all — same\n   shell}\n- {source: 'https://www.solo.io/security', http_status: 200, note: links to the trust center;\n   no certifications listed}\nrelated:\n  security_policy: https://www.solo.io/security\n  vulnerability_disclosure: security/solo-io-vulnerability-disclosure.yml\n  legal: https://legal.solo.io/\n  subprocessors: https://legal.solo.io/#subprocessors\n  dpa: https://legal.solo.io/#subscriber-dpa\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/security/solo-io-trust-center.yml
summary_line: trust center published
tags:
- Company
- API Gateway
- Service Mesh
- Kubernetes
- Istio
- Envoy
- AI Gateway
- Agentic AI
- Model Context Protocol
- Developer Portal
- Cloud Native
- Open Source
trust_url: https://trust.solo.io/
---
