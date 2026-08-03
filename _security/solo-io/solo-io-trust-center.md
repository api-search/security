---
api_specs:
- filename: solo-io-portal-server-openapi.yml
  format: yaml
  label: Gloo Portal Server API
  slug: portal-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-portal-server-openapi.yml
- filename: solo-io-portal-backend-openapi.yml
  format: yaml
  label: Gloo Portal Backend API
  slug: portal-backend
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-portal-backend-openapi.yml
- filename: solo-io-gloo-platform-portal-openapi.yml
  format: yaml
  label: Gloo Platform Portal API
  slug: gloo-platform-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-gloo-platform-portal-openapi.yml
- filename: solo-io-portal-idp-connect-openapi.yml
  format: yaml
  label: Gloo Portal IdP Connect API
  slug: portal-idp-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-portal-idp-connect-openapi.yml
- filename: solo-io-ai-gateway-guardrail-webhook-openapi.yml
  format: yaml
  label: AI Gateway Guardrail Webhook API
  slug: ai-guardrail-webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-ai-gateway-guardrail-webhook-openapi.yml
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
