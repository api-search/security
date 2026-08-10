---
certifications: []
description: ''
kind: trust-center
layout: security
name: Swiftly Trust Center
name_suffix: Trust Center
overview: Swiftly maintains a public trust center covering its security and compliance posture.
provider_name: Swiftly
provider_slug: swiftly
slug: swiftly-trust-center
source_filename: swiftly-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nprobe: true\nurl: https://trust.swiftly.com/\nplatform: Thoropass (formerly Laika) hosted Trust Center\ncertifications: []\ncertifications_note: >-\n  The trust center exists and returns HTTP 200 with <title>Trust Center</title>, but the\n  page is a client-side React SPA whose content is loaded from an AWS AppSync GraphQL\n  endpoint that rejects anonymous callers (HTTP 401 UnauthorizedException). No named\n  certification (SOC 2 / ISO 27001 / PCI DSS / HIPAA / GDPR) could be read without\n  executing JavaScript, so none are recorded here. Presence is confirmed; content is not.\n  Do not infer certifications from the presence of the trust center.\nevidence:\n- source: https://trust.swiftly.com/\n  http_status: 200\n  content_type: text/html; charset=utf-8\n  observed: '<title>Trust Center</title>; app bundle laika-app-prod.s3.amazonaws.com/static/trust-center/assets/index.js'\n- source: https://fhovr7cwmfgebommmcztmsw5ze.appsync-api.us-east-1.amazonaws.com/graphql\n\
  \  http_status: 401\n  observed: 'UnauthorizedException — trust center content API is not anonymously readable'\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://trust.swiftly.com/\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swiftly/refs/heads/main/security/swiftly-trust-center.yml
summary_line: trust center published
tags:
- Retail
- Retail Media
- Grocery
- Advertising
- Loyalty
- Coupons
- Commerce
- Artificial Intelligence
- Mobile
- Company
trust_url: https://trust.swiftly.com/
---
