---
api_specs:
- filename: lumos-tasks-api-openapi.yml
  format: yaml
  label: Lumos Tasks API
  slug: lumos-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-tasks-api-openapi.yml
- filename: lumos-access-reviews-api-openapi.yml
  format: yaml
  label: Lumos Access Reviews API
  slug: lumos-access-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-access-reviews-api-openapi.yml
- filename: lumos-core-api-openapi.yml
  format: yaml
  label: Lumos Core API
  slug: lumos-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-core-api-openapi.yml
- filename: lumos-integration-webhooks-api-openapi.yml
  format: yaml
  label: Lumos Integration Webhooks API
  slug: lumos-integration-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-integration-webhooks-api-openapi.yml
- filename: lumos-knowledge-api-openapi.yml
  format: yaml
  label: Lumos Knowledge API
  slug: lumos-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-knowledge-api-openapi.yml
- filename: lumos-lifecycle-management-api-openapi.yml
  format: yaml
  label: Lumos Lifecycle Management API
  slug: lumos-lifecycle-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-lifecycle-management-api-openapi.yml
- filename: lumos-meta-api-openapi.yml
  format: yaml
  label: Lumos Meta API
  slug: lumos-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-meta-api-openapi.yml
- filename: lumos-vendor-management-api-openapi.yml
  format: yaml
  label: Lumos Vendor Management API
  slug: lumos-vendor-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-vendor-management-api-openapi.yml
- filename: lumos-app-store-api-openapi.yml
  format: yaml
  label: Lumos App Store API
  slug: lumos-app-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-app-store-api-openapi.yml
certification_count: 0
certifications: []
description: Lumos runs a public trust centre at trust.lumos.com, hosted on Vanta. www.lumos.com/security redirects there, so it is the company's canonical security posture page.
kind: trust-center
layout: security
name: Lumos Trust Center
name_suffix: Trust Center
overview: Lumos maintains a public trust center covering its security and compliance posture.
provider_name: Lumos
provider_slug: lumos
slug: lumos-trust-center
source_filename: lumos-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://trust.lumos.com/\ndescription: >-\n  Lumos runs a public trust centre at trust.lumos.com, hosted on Vanta. www.lumos.com/security\n  redirects there, so it is the company's canonical security posture page.\ntrust_center:\n  url: https://trust.lumos.com/\n  platform: Vanta Trust Center\n  verified:\n    http_status: 200\n    probed: '2026-08-29'\n  redirect_from: https://www.lumos.com/security\ncertifications: []\ncertifications_note: >-\n  NO certification is asserted here. The Vanta trust centre is a client-rendered single-page app — the\n  served HTML is 7,466 bytes of bootstrap with no certification names in it, and the Vanta backend\n  proxy is not reachable anonymously. Certifications may well be listed to a human with a browser;\n  they are not machine-readable, so nothing was recorded. This is an `unreadable` surface, not an\n  absent one.\nevidence:\n- url: https://trust.lumos.com/\n  status: 200\n  note: 7,466-byte\
  \ Vanta SPA shell; zero occurrences of SOC, ISO, HIPAA, GDPR, PCI or FedRAMP in the body.\n- url: https://www.lumos.com/security\n  status: 200\n  note: Redirects to https://trust.lumos.com/.\nsecurity_contact:\n  email: security@lumos.com\n  source: PyPI package metadata for connector-py (author_email \"teamlumos <security@lumos.com>\")\n  note: >-\n    Recorded as an observed contact address, NOT as a published vulnerability disclosure policy —\n    Lumos serves no /.well-known/security.txt on any host and publishes no disclosure or bug-bounty\n    page that could be found. No VulnerabilityDisclosure artifact was written and no `Security`\n    pointer was emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/security/lumos-trust-center.yml
summary_line: trust center published
tags:
- Access Management
- Access Reviews
- Deprovisioning
- Identity Governance
- Identity Platform
- Least Privilege
- Provisioning
- SaaS Management
- Shadow IT
trust_url: ''
---
