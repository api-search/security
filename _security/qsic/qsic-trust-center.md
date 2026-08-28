---
certifications: []
description: ''
kind: trust-center
layout: security
name: Qsic Trust Center
name_suffix: Trust Center
overview: Qsic maintains a public trust center covering its security and compliance posture.
provider_name: Qsic
provider_slug: qsic
slug: qsic-trust-center
source_filename: qsic-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://trust.getqsic.com/\nprovider: Qsic\ntrust_center:\n  present: true\n  url: https://trust.getqsic.com/\n  title: QSIC Trust Center\n  platform: Vanta\n  platform_evidence: >-\n    Page is served from Vanta's trust-report bundle (assets.vanta.com/static/index-trust-report-*.js)\n    and carries data-slugid \"ea9fogyexwba0chwxwskxx\"; the tenant's Vanta region is app.aus.vanta.com\n    (Australia), consistent with Qsic being an Australian-headquartered company.\n  http_status: 200\n  content_type: text/html\n  fetched: '2026-08-26'\ncertifications: []\ncertifications_readable: false\ncertifications_note: >-\n  The trust center EXISTS and is publicly reachable, but its contents are not machine-readable. The\n  served HTML is a 5,435-byte single-page-app shell whose only text is the title \"QSIC Trust Center\";\n  every framework, control and document is fetched client-side from Vanta's GraphQL API, which\n  rejects anonymous\
  \ requests with {\"code\":\"BAD_REQUEST\",\"message\":\"Missing `signature` or\n  `signedAt`\"}. No certification (SOC 2, ISO 27001, PCI, HIPAA, FedRAMP, GDPR) could therefore be\n  read or verified, and NO `Compliance` pointer is emitted from this file — asserting certifications\n  we could not read would be fabrication.\nprobes:\n- url: https://trust.getqsic.com/\n  status: 200\n  note: Vanta trust center SPA shell.\n- url: https://app.aus.vanta.com/graphql\n  status: 400\n  note: 'Anonymous GraphQL rejected: Missing `signature` or `signedAt`.'\n- url: https://api.vanta.com/v1/trust-centers/ea9fogyexwba0chwxwskxx\n  status: 401\n  note: Unauthorized.\nremediation_for_provider: >-\n  Vanta trust centers can be configured to expose a public, crawlable summary of frameworks and\n  certifications. Serving the framework list as static HTML (or publishing a /.well-known/security.txt\n  that points at the trust center) would make the compliance posture readable to buyers, crawlers and\n  agents\
  \ rather than to browsers only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qsic/refs/heads/main/security/qsic-trust-center.yml
summary_line: trust center published
tags:
- Company
- Retail Media
- In-Store Audio
- Advertising
- Audio
- Retail
- Music
- Media
- Marketing
- Advertising Technology
trust_url: ''
---
