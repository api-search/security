---
api_specs:
- filename: ahasend-accounts-api-openapi.yml
  format: yaml
  label: AhaSend Accounts API
  slug: ahasend-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-accounts-api-openapi.yml
- filename: ahasend-api-keys-api-openapi.yml
  format: yaml
  label: AhaSend API Keys API
  slug: ahasend-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-api-keys-api-openapi.yml
- filename: ahasend-domains-api-openapi.yml
  format: yaml
  label: AhaSend Domains API
  slug: ahasend-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-domains-api-openapi.yml
- filename: ahasend-email-api-openapi.yml
  format: yaml
  label: AhaSend Email API
  slug: ahasend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-email-api-openapi.yml
- filename: ahasend-messages-api-openapi.yml
  format: yaml
  label: AhaSend Messages API
  slug: ahasend-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-messages-api-openapi.yml
- filename: ahasend-routes-api-openapi.yml
  format: yaml
  label: AhaSend Routes API
  slug: ahasend-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-routes-api-openapi.yml
- filename: ahasend-smtp-credentials-api-openapi.yml
  format: yaml
  label: AhaSend SMTP Credentials API
  slug: ahasend-smtp-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-smtp-credentials-api-openapi.yml
- filename: ahasend-statistics-api-openapi.yml
  format: yaml
  label: AhaSend Statistics API
  slug: ahasend-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-statistics-api-openapi.yml
- filename: ahasend-suppressions-api-openapi.yml
  format: yaml
  label: AhaSend Suppressions API
  slug: ahasend-suppressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-suppressions-api-openapi.yml
- filename: ahasend-utility-api-openapi.yml
  format: yaml
  label: AhaSend Utility API
  slug: ahasend-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-utility-api-openapi.yml
- filename: ahasend-webhooks-api-openapi.yml
  format: yaml
  label: AhaSend Webhooks API
  slug: ahasend-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-webhooks-api-openapi.yml
- filename: ahasend-sub-accounts-api-openapi.yml
  format: yaml
  label: AhaSend Sub Accounts API
  slug: ahasend-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/openapi/ahasend-sub-accounts-api-openapi.yml
certifications:
- GDPR
- Certified Senders Alliance (CSA)
- ISO/IEC 27001
- SOC 2
description: ''
kind: trust-center
layout: security
name: Ahasend Trust Center
name_suffix: Trust Center
overview: AhaSend maintains a public trust center documenting GDPR, Certified Senders Alliance (CSA), ISO/IEC 27001, and SOC 2 compliance.
provider_name: AhaSend
provider_slug: ahasend
slug: ahasend-trust-center
source_filename: ahasend-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nprobe: true\nsource: https://ahasend.com/trust\nurl: https://ahasend.com/trust\ncertifications:\n- name: GDPR\n  status: compliant\n  evidence: Dutch entity (AhaSend B.V., KvK 99533111) with a public Article 28 DPA at https://ahasend.com/dpa naming its three subprocessors.\n- name: Certified Senders Alliance (CSA)\n  status: certified\n  evidence: 'https://certified-senders.org/certificate/?id=8527228af85c77463bc7668b7d4f628f'\n- name: ISO/IEC 27001\n  status: in-progress\n  certified: false\n  evidence: >-\n    NOT CERTIFIED. AhaSend states the certification audit is scheduled for September 2026 and\n    labels the badge \"in progress\"/\"pending\" on its own pages. Corrected by hand on 2026-08-30\n    after the automated probe recorded the keyword match as a certification.\n- name: SOC 2\n  status: none\n  certified: false\n  evidence: No SOC 2 report or attestation is published or claimed.\nevidence:\n- source: https://ahasend.com/trust\n\
  \  keywords:\n  - iso 27001\n  - trust center\n  - gdpr\ndata_residency:\n  region: EU/EEA\n  sites: 5 sites across 4 countries (Falkenstein, Nuremberg, Helsinki, Oslo, Sofia)\n  note: >-\n    All email content, message data, metadata, logs and analytics are stated to stay within the\n    EU/EEA on hardware AhaSend owns. Two disclosed exceptions: ahasend.com's nameservers are\n    currently at Cloudflare (website DNS, not email data; migration stated as planned), and an\n    optional US egress/SMTP node in Hillsboro, Oregon that is opt-in and off by default.\nsubprocessors:\n  published: true\n  location: https://ahasend.com/dpa\n  named: [Hetzner, DA International Group Ltd, Blix]\npages:\n  security_overview: https://ahasend.com/security\n  dpa: https://ahasend.com/dpa\n  responsible_disclosure: https://ahasend.com/responsible-disclosure\n  status: https://status.ahasend.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/security/ahasend-trust-center.yml
summary_line: GDPR, Certified Senders Alliance (CSA), ISO/IEC 27001, SOC 2
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhook
trust_url: https://ahasend.com/trust
---
