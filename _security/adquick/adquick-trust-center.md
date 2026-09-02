---
certifications: []
description: ''
kind: trust-center
layout: security
name: Adquick Trust Center
name_suffix: Trust Center
overview: AdQuick maintains a public trust center covering its security and compliance posture.
provider_name: AdQuick
provider_slug: adquick
slug: adquick-trust-center
source_filename: adquick-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://trust.adquick.com/\nnotes: >-\n  AdQuick operates a public Trust Center at trust.adquick.com, hosted on Vanta\n  (DNS CNAME -> 66d814094617356976de24c6.cname.vantatrust.com). It is the only AdQuick web property\n  outside api.adquick.com that answers an automated request: www., docs., help. and blog.adquick.com\n  all return a Cloudflare 403 bot challenge. The Trust Center returns HTTP 200 with a real Vanta\n  trust-report document (title \"AdQuick Trust Center\", canonical https://trust.adquick.com), but the\n  control/certification list is rendered client-side from Vanta's GraphQL API, which rejects\n  unauthenticated calls (\"Missing `signature` or `signedAt`\"). NAMED CERTIFICATIONS COULD THEREFORE\n  NOT BE READ, and none are asserted here. No `Compliance` pointer is emitted for that reason - the\n  trust center is verified present, its certification set is not.\ntrust_center:\n  url: https://trust.adquick.com/\n\
  \  title: AdQuick Trust Center\n  platform: Vanta\n  platform_evidence: >-\n    content-location https://assets.vanta.com/static/vite/index-trust-report.vite...html;\n    DNS CNAME 66d814094617356976de24c6.cname.vantatrust.com\n  public: true\n  access_request_required_for_documents: unknown\ncertifications: []\ncertifications_readable: false\ncertifications_blocker: >-\n  Vanta trust-report content is JS-rendered; the backing GraphQL endpoint (app.vanta.com/graphql)\n  requires a signed request and returns 400 to anonymous clients.\nsecurity_posture_statements:\n- source: https://trust.adquick.com/ (meta description, served in HTML)\n  text: >-\n    \"At AdQuick, we are committed to ensuring the highest standards of security and trust for our\n    users. As a leader in OOH advertising, we take the responsibility of safeguarding your data and\n    maintaining confidentiality very seriously.\"\n  note: marketing statement only; not a certification claim\ntransport_security:\n  hsts: 'max-age=31536000;\
  \ includeSubDomains'\n  observed_on: trust.adquick.com\n  note: >-\n    HSTS is present on the Vanta-hosted trust host but was NOT observed on www., docs. or\n    api.adquick.com (see security/adquick-domain-security.yml).\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://trust.adquick.com/\n  http_status: 200\n  content_type: text/html\n  cf_ray: a2a988ca1ff56a56-EWR\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adquick/refs/heads/main/security/adquick-trust-center.yml
summary_line: trust center published
tags:
- Company
- Enterprise Saas
- Advertising
- Out-of-Home Advertising
- DOOH
- Programmatic Advertising
- Media Buying
- Marketing
- MCP
trust_url: ''
---
