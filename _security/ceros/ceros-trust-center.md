---
api_specs:
- filename: ceros-accounts-api-openapi.yml
  format: yaml
  label: Ceros Accounts API
  slug: ceros-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-accounts-api-openapi.yml
- filename: ceros-embedcodes-api-openapi.yml
  format: yaml
  label: Ceros Embed Codes API
  slug: ceros-embedcodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-embedcodes-api-openapi.yml
- filename: ceros-experience-api-openapi.yml
  format: yaml
  label: Ceros Experience API
  slug: ceros-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-experience-api-openapi.yml
- filename: ceros-experiencepage-api-openapi.yml
  format: yaml
  label: Ceros Experience Page API
  slug: ceros-experiencepage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-experiencepage-api-openapi.yml
- filename: ceros-folders-api-openapi.yml
  format: yaml
  label: Ceros Folders API
  slug: ceros-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-folders-api-openapi.yml
- filename: ceros-oembed-api-openapi.yml
  format: yaml
  label: Ceros Oembed API
  slug: ceros-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/openapi/ceros-oembed-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Ceros Trust Center
name_suffix: Trust Center
overview: Ceros maintains a public trust center covering its security and compliance posture.
provider_name: Ceros
provider_slug: ceros
slug: ceros-trust-center
source_filename: ceros-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://trust.ceros.com/\nprovider: Ceros\ntrust_center:\n  url: https://trust.ceros.com/\n  platform: Vanta\n  slug_id: 9ldxavzelo7uuybddceynn\n  title: Ceros Trust Center\n  tagline: >-\n    \"Security is built into the fabric of our products, team, infrastructure, and processes, so\n    you can rest assured your data is safeguarded.\"\n  x-evidence:\n    fetched: '2026-08-09'\n    url: https://trust.ceros.com/\n    http_status: 200\n    content_type: text/html\n    bytes: 6622\ncertifications: []\ncertifications_note: >-\n  NONE RECORDED, DELIBERATELY. The trust centre is a client-side Vanta SPA: the served HTML is a\n  6,622-byte shell carrying only the title and description, and every /api/* path under\n  trust.ceros.com and app.vanta.com returns that same shell with a 200 rather than JSON — a\n  soft-404, not data. No certification, attestation or audit report name was readable, so none is\n  asserted here and no `Compliance`\
  \ pointer is emitted in apis.yml. A trust centre that only\n  renders in a browser is not a machine-readable compliance posture.\n  control_probe:\n  - url: https://trust.ceros.com/api/trust-page\n    http_status: 200\n    bytes: 6402\n    verdict: SPA catch-all — identical shell, no JSON.\n  - url: https://app.vanta.com/api/trust-page/9ldxavzelo7uuybddceynn\n    http_status: 200\n    bytes: 29762\n    verdict: SPA catch-all.\n  - url: https://api.vanta.com/trust/9ldxavzelo7uuybddceynn\n    http_status: 401\nreadable_security_claims:\n  source: https://www.ceros.com/technical-faq-s/\n  claims:\n  - topic: TLS\n    claim: >-\n      \"Secure TLS connections are used for all logged in sessions. We support secure connections\n      for published Experience content but do not force it.\"\n  - topic: SSO\n    claim: >-\n      \"Ceros supports both password authentication and enterprise SSO using identity standards:\n      LDAP, SAML, and OAuth.\"\n  - topic: Access control\n    claim: Account\
  \ Owner and Member roles, with project-level access restrictions available.\n  - topic: Hosting\n    claim: >-\n      Published experience content, media and assets served from S3 with CloudFront and Cloudflare\n      in front as CDNs; Admin and Studio served from Ceros-managed AWS EC2 instances.\n  note: >-\n    This readable page names no certification either — no SOC 2, ISO 27001, PCI, HIPAA, FedRAMP,\n    GDPR or CCPA claim appears on it.\nvulnerability_disclosure:\n  published: false\n  probes:\n  - url: https://www.ceros.com/.well-known/security.txt\n    http_status: 404\n  - url: https://developers.ceros.com/.well-known/security.txt\n    http_status: 404\n  - url: https://rest.ceros.com/.well-known/security.txt\n    http_status: 404\n  - url: https://www.ceros.com/security/\n    http_status: 404\n  false_positive_avoided:\n    url: https://educate.ceros.com/.well-known/security.txt\n    http_status: 200\n    reason: >-\n      Served from a Ceros CNAME but it is Intercom's policy\
  \ — Contact bugcrowd.com/intercom,\n      Canonical https://app.intercom.com/.well-known/security.txt. It is the help-centre vendor's\n      programme, not Ceros's, so it is NOT credited to Ceros and no `Security` pointer is emitted.\n  only_published_security_address:\n    value: mailto:domains@ceros.com\n    source: 'CAA record iodef for ceros.com'\n    note: A certificate-authority incident-reporting address, not a vulnerability disclosure contact.\n  remedy: >-\n    Publish /.well-known/security.txt on www.ceros.com and rest.ceros.com with a Contact and\n    Policy, per RFC 9116. Ceros already runs a Vanta trust centre — the disclosure channel is the\n    one thing it does not expose at a fetchable URL.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceros/refs/heads/main/security/ceros-trust-center.yml
summary_line: trust center published
tags:
- Content Management
- Interactive Content
- Digital Experience
- Embed
- oEmbed
- CMS Integration
- Marketing
- Design
- No-Code
- Content Delivery
- Media and Publishing
- SDK
trust_url: ''
---
