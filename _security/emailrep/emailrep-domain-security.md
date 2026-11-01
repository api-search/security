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
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emailrep.io
  spf: false
hosts:
- cert_expires: Oct 19 21:43:22 2026 GMT
  host: emailrep.io
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Emailrep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EmailRep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: EmailRep
provider_slug: emailrep
slug: emailrep-domain-security
source_filename: emailrep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emailrep.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 19 21:43:22 2026 GMT\n  hsts: null\ndomains:\n- domain: emailrep.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/emailrep/security/emailrep-domain-security.yml
summary_line: TLSv1.2 · DMARC
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
---
