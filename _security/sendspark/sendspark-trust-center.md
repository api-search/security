---
api_specs:
- filename: sendspark-dvm-bundles-api-openapi.yml
  format: yaml
  label: Sendspark DVM Bundles API
  slug: sendspark-dvm-bundles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/openapi/sendspark-dvm-bundles-api-openapi.yml
- filename: sendspark-dynamics-campaign-api-openapi.yml
  format: yaml
  label: Sendspark Dynamics Campaign API
  slug: sendspark-dynamics-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/openapi/sendspark-dynamics-campaign-api-openapi.yml
- filename: sendspark-webhook-api-openapi.yml
  format: yaml
  label: Sendspark Webhook API
  slug: sendspark-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/openapi/sendspark-webhook-api-openapi.yml
- filename: sendspark-workspace-api-openapi.yml
  format: yaml
  label: Sendspark Workspace API
  slug: sendspark-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/openapi/sendspark-workspace-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Sendspark Trust Center
name_suffix: Trust Center
overview: Sendspark maintains a public trust center covering its security and compliance posture.
provider_name: Sendspark
provider_slug: sendspark
slug: sendspark-trust-center
source_filename: sendspark-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nprobe: true\nurl: https://security.sendspark.com/\npresent: true\ncertifications: []\ncertifications_readable: false\nplatform: Laika (trust-center SPA)\nevidence:\n- source: https://security.sendspark.com/\n  http_status: 200\n  content_type: text/html; charset=utf-8\n  title: Trust Center\n  bundle: https://laika-app-prod.s3.amazonaws.com/static/trust-center/assets/index.js\n  note: >-\n    An 814-byte HTML shell with a single <div id=\"root\"> hydrated by the Laika\n    trust-center JavaScript bundle. The <title> is \"Trust Center\" and the asset\n    host is unambiguously a trust-center product, so the surface genuinely\n    exists on a subdomain Sendspark controls — but every certification, policy\n    and subprocessor listing is rendered client-side and returned no readable\n    text to an HTTP fetch.\nnegative_probes:\n- {url: 'https://trust.sendspark.com', status: 0, note: DNS/connection failure — no such host}\n- {url: 'https://www.sendspark.com/security',\
  \ status: 404}\n- {url: 'https://www.sendspark.com/trust', status: 404}\n- {url: 'https://www.sendspark.com/security-and-compliance', status: 404}\n- {url: 'https://www.sendspark.com/gdpr', status: 404}\n- {url: 'https://www.sendspark.com/legal', status: 404}\n- {url: 'https://www.sendspark.com/dpa', status: 404}\n- {url: 'https://www.sendspark.com/sub-processors', status: 404}\nfindings:\n- >-\n  Sendspark operates a trust center at security.sendspark.com, but it is not\n  linked from the sendspark.com footer (which links only /privacy and /terms)\n  and it is not discoverable from the docs. A buyer or an agent looking for\n  Sendspark's compliance posture has no path to it from the public site.\n- >-\n  NO named certification (SOC 2, ISO 27001, PCI DSS, HIPAA, FedRAMP, GDPR, CSA\n  STAR) could be confirmed from any machine-readable surface. This artifact\n  records the presence of the trust center, NOT a compliance claim — no\n  `Compliance` pointer is emitted, because nothing verifiable\
  \ was published in\n  a form a machine can read.\nremediation_for_provider:\n- Link security.sendspark.com from the sendspark.com footer and from help.sendspark.com.\n- Publish a server-rendered or JSON summary of certifications so the trust center is machine-readable.\n- Serve a /.well-known/security.txt (RFC 9116) — no Sendspark host serves one today.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendspark/refs/heads/main/security/sendspark-trust-center.yml
summary_line: trust center published
tags:
- Company
- Video
- Sales
- Marketing
- Personalization
- Artificial Intelligence
- Video Messaging
- Webhook
- MCP
trust_url: https://security.sendspark.com/
---
