---
api_specs:
- filename: lumos-openapi.json
  format: json
  label: Lumos REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-openapi.json
- filename: lumos-accesspolicies-api-openapi.yml
  format: yaml
  label: Lumos AccessPolicies API
  slug: lumos-accesspolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accesspolicies-api-openapi.yml
- filename: lumos-accessrequests-api-openapi.yml
  format: yaml
  label: Lumos AccessRequests API
  slug: lumos-accessrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accessrequests-api-openapi.yml
- filename: lumos-accessreviews-api-openapi.yml
  format: yaml
  label: Lumos AccessReviews API
  slug: lumos-accessreviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accessreviews-api-openapi.yml
- filename: lumos-accounts-api-openapi.yml
  format: yaml
  label: Lumos Accounts API
  slug: lumos-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accounts-api-openapi.yml
- filename: lumos-activity-api-openapi.yml
  format: yaml
  label: Lumos Activity API
  slug: lumos-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-activity-api-openapi.yml
- filename: lumos-apps-api-openapi.yml
  format: yaml
  label: Lumos Apps API
  slug: lumos-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-apps-api-openapi.yml
- filename: lumos-appstore-api-openapi.yml
  format: yaml
  label: Lumos AppStore API
  slug: lumos-appstore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-appstore-api-openapi.yml
- filename: lumos-groups-api-openapi.yml
  format: yaml
  label: Lumos Groups API
  slug: lumos-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-groups-api-openapi.yml
- filename: lumos-preapprovalrules-api-openapi.yml
  format: yaml
  label: Lumos PreApprovalRules API
  slug: lumos-preapprovalrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-preapprovalrules-api-openapi.yml
- filename: lumos-tasks-api-openapi.yml
  format: yaml
  label: Lumos Tasks API
  slug: lumos-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-tasks-api-openapi.yml
- filename: lumos-users-api-openapi.yml
  format: yaml
  label: Lumos Users API
  slug: lumos-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-users-api-openapi.yml
- filename: lumos-utility-api-openapi.yml
  format: yaml
  label: Lumos Utility API
  slug: lumos-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-utility-api-openapi.yml
- filename: lumos-vendors-api-openapi.yml
  format: yaml
  label: Lumos Vendors API
  slug: lumos-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-vendors-api-openapi.yml
- filename: lumos-webhooks-api-openapi.yml
  format: yaml
  label: Lumos Webhooks API
  slug: lumos-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-webhooks-api-openapi.yml
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
