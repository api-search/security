---
api_specs:
- filename: umami-authentication-api-openapi.yml
  format: yaml
  label: Umami Authentication API
  slug: umami-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-authentication-api-openapi.yml
- filename: umami-events-api-openapi.yml
  format: yaml
  label: Umami Events API
  slug: umami-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-events-api-openapi.yml
- filename: umami-sessions-api-openapi.yml
  format: yaml
  label: Umami Sessions API
  slug: umami-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-sessions-api-openapi.yml
- filename: umami-teams-api-openapi.yml
  format: yaml
  label: Umami Teams API
  slug: umami-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-teams-api-openapi.yml
- filename: umami-users-api-openapi.yml
  format: yaml
  label: Umami Users API
  slug: umami-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-users-api-openapi.yml
- filename: umami-website-statistics-api-openapi.yml
  format: yaml
  label: Umami Website Statistics API
  slug: umami-website-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-website-statistics-api-openapi.yml
- filename: umami-websites-api-openapi.yml
  format: yaml
  label: Umami Websites API
  slug: umami-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-websites-api-openapi.yml
certifications: []
description: Umami publishes a detailed security page covering privacy-by-design, encryption, access control, secure development, infrastructure, incident response, data retention/deletion and responsible disclosure. It also publishes an unusually honest assurance table that states plainly what it has NOT certified.
kind: trust-center
layout: security
name: Umami Trust Center
name_suffix: Trust Center
overview: Umami maintains a public trust center covering its security and compliance posture.
provider_name: Umami
provider_slug: umami
slug: umami-trust-center
source_filename: umami-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://umami.is/security\nurl: https://umami.is/security\nprovider: Umami\nproviderId: umami\ndescription: >-\n  Umami publishes a detailed security page covering privacy-by-design,\n  encryption, access control, secure development, infrastructure, incident\n  response, data retention/deletion and responsible disclosure. It also\n  publishes an unusually honest assurance table that states plainly what it has\n  NOT certified.\ncorrection: >-\n  The automated probe (probe-security-programs.py) matched the strings \"SOC 2\"\n  and \"ISO 27001\" on this page and recorded them as certifications. That was\n  keyword matching, not reading: the page names both only to say \"Not currently\n  certified\". This file was corrected by hand on 2026-08-13. Umami holds no\n  third-party security certification and has not completed an independent\n  penetration test.\ncertifications: []\ncertifications_explicitly_denied:\n  - name: SOC 2\n\
  \    status: Not currently certified\n  - name: ISO 27001\n    status: Not currently certified\n  - name: Independent penetration test\n    status: Not yet completed\ncompliance:\n  - name: GDPR\n    status: claimed\n    detail: >-\n      \"Umami is designed to support compliant analytics use.\" Umami does not use\n      cookies, does not collect directly identifying information, and does not\n      track visitors across sites, so it states no cookie consent banner is\n      required.\n  - name: CCPA\n    status: claimed\n    detail: Same posture as GDPR; stated on both the security and pricing pages.\n  - name: Data Processing Agreement\n    status: published\n    url: https://umami.is/dpa\n    detail: Publicly available without a sales conversation.\n  - name: PCI\n    status: delegated\n    detail: >-\n      Payments are processed by Stripe. Umami states it does not directly store\n      complete payment-card numbers or card security codes.\n  - name: Open-source review\n    status:\
  \ published\n    detail: >-\n      Source code publicly available under MIT at\n      https://github.com/umami-software/umami — offered on the security page as\n      a substitute form of independent review.\ndata_residency:\n  available: true\n  regions: [us, eu]\n  detail: >-\n    Geographic data-region selection for Umami Cloud accounts. The API honors it\n    as a path segment — https://api.umami.is/v1/us and https://api.umami.is/v1/eu\n    — defaulting to the region of the account that owns the key.\npractices_published:\n  encryption_in_transit: HTTPS with industry-standard TLS.\n  encryption_at_rest: >-\n    Delegated to infrastructure and database providers that support encryption\n    at rest; backups protected by the applicable provider's controls.\n  secrets: Production credentials stored separately from source; access restricted.\n  tenancy: >-\n    Logical separation of customer accounts, teams, websites and analytics data,\n    enforced by application authorization controls.\n\
  \  access_control:\n    - Individual accounts rather than shared production credentials\n    - Least-privilege permissions\n    - Multi-factor authentication on critical services where supported\n    - Restricted administrative and production access\n    - Access removal when no longer required\n  sdlc:\n    - Peer review of material code changes\n    - Automated testing\n    - Dependency and vulnerability monitoring\n    - Regular dependency and security updates\n    - Separation of development and production environments\n    - Investigation of reported vulnerabilities and GitHub security advisories\n  incident_response: >-\n    Documented process. Umami commits to notifying affected customers without\n    unreasonable delay when a confirmed incident affects customer data, by\n    email, in-app, or via the service-status page.\n  availability: >-\n    No uptime guarantee outside the Enterprise plan, which lists an Uptime SLA.\n    Status published at https://umami.statuspage.io.\ncustomer_security_review:\
  \ >-\n    \"Security questionnaires and additional information may be provided during a\n    legitimate customer procurement or security review.\" Contact via\n    https://umami.is/contact.\nstated_direction: >-\n  \"We are evaluating formal compliance programs and an independent third-party\n  penetration test as Umami Cloud and its enterprise customer base grow.\"\ncontacts:\n  security: security@umami.is\n  privacy: privacy@umami.is\n  support: support@umami.is\n  sales: sales@umami.is\nrelated:\n  - https://umami.is/privacy\n  - https://umami.is/dpa\n  - https://umami.statuspage.io\nevidence:\n  - url: https://umami.is/security\n    status: 200\n    note: >-\n      Body is streamed as a Next.js RSC flight payload; read from the payload\n      rather than the initial HTML shell, which contains only the page title.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/security/umami-trust-center.yml
summary_line: trust center published
tags:
- Cookieless Tracking
- Open-Source
- Privacy
- Web Analytics
- Website Analytics
- Product Analytics
- Event Tracking
- Self-Hosted
- GDPR
- Session Replay
- Heatmaps
- Marketing Attribution
trust_url: https://umami.is/security
---
