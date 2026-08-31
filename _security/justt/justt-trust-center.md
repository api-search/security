---
api_specs:
- filename: justt-chargebacks-api-openapi.yml
  format: yaml
  label: Justt Chargebacks API
  slug: justt-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-chargebacks-api-openapi.yml
- filename: justt-data-subjects-api-openapi.yml
  format: yaml
  label: Justt Data Subjects API
  slug: justt-data-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-data-subjects-api-openapi.yml
- filename: justt-evidence-api-openapi.yml
  format: yaml
  label: Justt Evidence API
  slug: justt-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-evidence-api-openapi.yml
- filename: justt-files-api-openapi.yml
  format: yaml
  label: Justt Files API
  slug: justt-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-files-api-openapi.yml
- filename: justt-integrations-api-openapi.yml
  format: yaml
  label: Justt Integrations API
  slug: justt-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-integrations-api-openapi.yml
- filename: justt-merchants-api-openapi.yml
  format: yaml
  label: Justt Merchants API
  slug: justt-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-merchants-api-openapi.yml
- filename: justt-pre-chargeback-alerts-api-openapi.yml
  format: yaml
  label: Justt Pre-chargeback Alerts API
  slug: justt-pre-chargeback-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-pre-chargeback-alerts-api-openapi.yml
- filename: justt-sandbox-api-openapi.yml
  format: yaml
  label: Justt Sandbox API
  slug: justt-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-sandbox-api-openapi.yml
- filename: justt-transactions-api-openapi.yml
  format: yaml
  label: Justt Transactions API
  slug: justt-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/openapi/justt-transactions-api-openapi.yml
certifications:
- SOC 2 Type II
- ISO 27001
- ISO 27017
- ISO 27018
description: ''
kind: trust-center
layout: security
name: Justt Trust Center
name_suffix: Trust Center
overview: Justt maintains a public trust center documenting SOC 2 Type II, ISO 27001, ISO 27017, and ISO 27018 compliance.
provider_name: Justt
provider_slug: justt
slug: justt-trust-center
source_filename: justt-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nprobe: true\nurl: https://trust.justt.ai/\nplatform: Vanta\ncertifications:\n- SOC 2 Type II\n- ISO 27001\n- ISO 27017\n- ISO 27018\nregimes:\n- GDPR\n- CCPA\ndata_handling:\n- per-customer data isolation\nevidence:\n- source: https://trust.justt.ai/\n  http_status: 200\n  kind: trust-center\n  keywords: [trust, security, compliance]\n  markers:\n  - 'title: Justt Trust Center'\n  - 'canonical: https://trust.justt.ai'\n  - 'data-signature-manifest-url: https://assets.vanta.com/static/signature-manifest...'\n  - 'meta description: \"Use this Trust Center to learn about our security posture and\n    request access to our security documentation.\"'\n- source: https://justt.ai/\n  http_status: 200\n  kind: compliance-claim\n  quotes:\n  - SOC 2 Type II plus the full ISO 27001 family\n  - ISO 27001 / 27017 / 27018\n  - GDPR\n  - CCPA\n- source: openapi/justt-rest-api-openapi-original.json\n  kind: contract-backed-compliance\n  note: >-\n\
  \    POST /data-subjects/removal (DataSubjectsController_requestDataSubjectRemoval)\n    — \"Request to remove personal data from the Justt system in compliance with\n    data protection regulations (GDPR, CCPA).\" The erasure right is callable, not\n    just asserted.\naccess:\n  documents_public: false\n  note: >-\n    The certification reports themselves are request-gated behind the Vanta trust\n    center (\"request access to our security documentation\"), which is the normal\n    posture. The certification NAMES are public on justt.ai and are what is\n    recorded here.\nreadability_note: >-\n  trust.justt.ai is a client-rendered Vanta single-page app that answers 200 with\n  the same HTML shell for every path, so the automated keyword probe\n  (probe-security-programs.py) recorded no hit. This file was written from the\n  server-rendered head metadata plus the compliance claims on justt.ai's own\n  homepage, both fetched directly. The Vanta shell is why an automated scan of\n  this\
  \ trust center returns nothing.\nvulnerability_disclosure:\n  published: false\n  note: >-\n    Justt publishes no vulnerability disclosure route reachable without a browser\n    session. /.well-known/security.txt returns 404 on justt.ai, www.justt.ai,\n    api.justt.ai, app.justt.ai and developers.justt.ai; /security,\n    /security-policy and /responsible-disclosure all return 404 on justt.ai; and\n    no HackerOne, Bugcrowd or Intigriti programme was found. No\n    VulnerabilityDisclosure, Security or SecurityTxt pointer is emitted. Publishing\n    an RFC 9116 security.txt naming the existing trust-center contact would be a\n    one-file fix.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justt/refs/heads/main/security/justt-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, ISO 27017, ISO 27018
tags:
- Company
- Payments
- Chargebacks
- Disputes
- Fraud
- Risk
- Financial-Services
- E-Commerce
- Artificial Intelligence
- Webhook
trust_url: https://trust.justt.ai/
---
