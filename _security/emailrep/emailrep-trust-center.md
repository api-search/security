---
api_specs:
- filename: emailrep-binexplode-api-openapi.yml
  format: yaml
  label: EmailRep Bin Explode API
  slug: emailrep-binexplode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-binexplode-api-openapi.yml
- filename: emailrep-dlp-release-requests-api-openapi.yml
  format: yaml
  label: EmailRep DLP release requests API
  slug: emailrep-dlp-release-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-dlp-release-requests-api-openapi.yml
- filename: emailrep-email-bombs-api-openapi.yml
  format: yaml
  label: EmailRep Email Bombs API
  slug: emailrep-email-bombs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-email-bombs-api-openapi.yml
- filename: emailrep-enrichment-api-openapi.yml
  format: yaml
  label: EmailRep Enrichment API
  slug: emailrep-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-enrichment-api-openapi.yml
- filename: emailrep-events-in-the-audit-log-api-openapi.yml
  format: yaml
  label: EmailRep Events in the audit log API
  slug: emailrep-events-in-the-audit-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-events-in-the-audit-log-api-openapi.yml
- filename: emailrep-export-api-openapi.yml
  format: yaml
  label: EmailRep Export API
  slug: emailrep-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-export-api-openapi.yml
- filename: emailrep-hunt-jobs-api-openapi.yml
  format: yaml
  label: EmailRep Hunt Jobs API
  slug: emailrep-hunt-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-hunt-jobs-api-openapi.yml
- filename: emailrep-lists-api-openapi.yml
  format: yaml
  label: EmailRep Lists API
  slug: emailrep-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-lists-api-openapi.yml
- filename: emailrep-live-flow-api-openapi.yml
  format: yaml
  label: EmailRep Live flow API
  slug: emailrep-live-flow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-live-flow-api-openapi.yml
- filename: emailrep-mailboxes-api-openapi.yml
  format: yaml
  label: EmailRep Mailboxes API
  slug: emailrep-mailboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-mailboxes-api-openapi.yml
- filename: emailrep-message-groups-api-openapi.yml
  format: yaml
  label: EmailRep Message Groups API
  slug: emailrep-message-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-message-groups-api-openapi.yml
- filename: emailrep-messages-api-openapi.yml
  format: yaml
  label: EmailRep Messages API
  slug: emailrep-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-messages-api-openapi.yml
- filename: emailrep-reports-api-openapi.yml
  format: yaml
  label: EmailRep Reports API
  slug: emailrep-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-reports-api-openapi.yml
- filename: emailrep-reputation-api-openapi.yml
  format: yaml
  label: EmailRep Reputation API
  slug: emailrep-reputation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-reputation-api-openapi.yml
- filename: emailrep-roles-api-openapi.yml
  format: yaml
  label: EmailRep Roles API
  slug: emailrep-roles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-roles-api-openapi.yml
- filename: emailrep-rules-api-openapi.yml
  format: yaml
  label: EmailRep Rules API
  slug: emailrep-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-rules-api-openapi.yml
- filename: emailrep-scim-api-openapi.yml
  format: yaml
  label: EmailRep SCIM API
  slug: emailrep-scim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-scim-api-openapi.yml
- filename: emailrep-tasks-api-openapi.yml
  format: yaml
  label: EmailRep Tasks API
  slug: emailrep-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-tasks-api-openapi.yml
- filename: emailrep-user-reports-api-openapi.yml
  format: yaml
  label: EmailRep User Reports API
  slug: emailrep-user-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emailrep/openapi/emailrep-user-reports-api-openapi.yml
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Emailrep Trust Center
name_suffix: Trust Center
overview: EmailRep maintains a public trust center covering its security and compliance posture.
provider_name: EmailRep
provider_slug: emailrep
slug: emailrep-trust-center
source_filename: emailrep-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nprobe: true\nurl: https://trust.sublime.security/\nhttp_status: 200\ntitle: Sublime Security Trust Center\ncertifications: []\nownership:\n  justified: true\n  statement: >-\n    EmailRep is operated by Sublime Security, Inc. — emailrep.io's own footer reads \"Operated by\n    Sublime Security, Inc\" and links sublimesecurity.com/terms and /privacy — so the operator's\n    trust center is the trust surface that governs this API. It is a parent-brand page, not an\n    EmailRep-specific one.\ndetail: >-\n  The trust center exists and resolves (trust.sublimesecurity.com 301s to\n  trust.sublime.security, which returns HTTP 200 with the document title \"Sublime Security Trust\n  Center\"). It is rendered entirely client-side: the 4,961-byte anonymous response carries the\n  title and nothing else — no certification names, no controls, no subprocessor list, no security\n  contact. Two independent anonymous reads on 2026-08-13 (curl and a\
  \ rendering fetch) both\n  returned zero named frameworks.\n  Because NO certification could be verified anonymously, `certifications` is an empty list and\n  NO `Compliance` pointer is emitted in apis.yml. Recording the page as present without a\n  verified cert would credit a compliance posture that was not observed. This is a real finding\n  about the trust center, not a failure to look: a trust center that a machine cannot read is\n  a trust center that agents and procurement bots cannot use.\nevidence:\n  - source: https://trust.sublime.security/\n    http_status: 200\n    content_type: text/html\n    bytes: 4961\n    extractable_text: 'Sublime Security Trust Center'\n  - source: https://trust.sublimesecurity.com\n    http_status: 301\n    redirects_to: https://trust.sublime.security/\nvulnerability_disclosure:\n  found: false\n  detail: >-\n    No vulnerability-disclosure artifact is written and no `Security` pointer is emitted. Probed\n    on 2026-08-13: emailrep.io/.well-known/security.txt\
  \ 404, emailrep.io/security 404,\n    emailrep.io/responsible-disclosure 404, hackerone.com/sublime_security 404,\n    bugcrowd.com/sublimesecurity 404. sublime.security/security and\n    sublime.security/responsible-disclosure could not be read — that host answers every anonymous\n    request with HTTP 429 behind a Vercel Security Checkpoint, so their existence is unknown\n    rather than disproved.\nrelated:\n  - security/emailrep-domain-security.yml\n  - well-known/emailrep-well-known.yml\n"
source_yaml_url: https://artifacts.apis.io/emailrep/security/emailrep-trust-center.yml
summary_line: trust center published
tags:
- Security
- Email
- Email Reputation
- Threat Intelligence
- Phishing
- Fraud Prevention
- Anti-Abuse
- Deliverability
- Risk Scoring
- Public APIs
trust_url: https://trust.sublime.security/
---
