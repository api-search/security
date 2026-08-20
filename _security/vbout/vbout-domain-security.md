---
api_specs:
- filename: vbout-account-api-openapi.yml
  format: yaml
  label: VBOUT Account API
  slug: vbout-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-account-api-openapi.yml
- filename: vbout-aichatbot-api-openapi.yml
  format: yaml
  label: VBOUT AIchatbot API
  slug: vbout-aichatbot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-aichatbot-api-openapi.yml
- filename: vbout-application-api-openapi.yml
  format: yaml
  label: VBOUT Application API
  slug: vbout-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-application-api-openapi.yml
- filename: vbout-automation-api-openapi.yml
  format: yaml
  label: VBOUT Automation API
  slug: vbout-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-automation-api-openapi.yml
- filename: vbout-contact-api-openapi.yml
  format: yaml
  label: VBOUT Contact API
  slug: vbout-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-contact-api-openapi.yml
- filename: vbout-email-marketing-api-openapi.yml
  format: yaml
  label: VBOUT Email Marketing API
  slug: vbout-email-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-email-marketing-api-openapi.yml
- filename: vbout-emailmarketing-api-openapi.yml
  format: yaml
  label: VBOUT EmailMarketing API
  slug: vbout-emailmarketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-emailmarketing-api-openapi.yml
- filename: vbout-goals-api-openapi.yml
  format: yaml
  label: VBOUT Goals API
  slug: vbout-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-goals-api-openapi.yml
- filename: vbout-help-api-openapi.yml
  format: yaml
  label: VBOUT Help API
  slug: vbout-help-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-help-api-openapi.yml
- filename: vbout-pipeline-api-openapi.yml
  format: yaml
  label: VBOUT Pipeline API
  slug: vbout-pipeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-pipeline-api-openapi.yml
- filename: vbout-popups-api-openapi.yml
  format: yaml
  label: VBOUT Popups API
  slug: vbout-popups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-popups-api-openapi.yml
- filename: vbout-settings-api-openapi.yml
  format: yaml
  label: VBOUT Settings API
  slug: vbout-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-settings-api-openapi.yml
- filename: vbout-social-media-api-openapi.yml
  format: yaml
  label: VBOUT Social Media API
  slug: vbout-social-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-social-media-api-openapi.yml
- filename: vbout-socialmedia-api-openapi.yml
  format: yaml
  label: VBOUT SocialMedia API
  slug: vbout-socialmedia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-socialmedia-api-openapi.yml
- filename: vbout-users-workflow-api-openapi.yml
  format: yaml
  label: VBOUT Users & Workflow API
  slug: vbout-users-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/openapi/vbout-users-workflow-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vbout.com
  spf: true
hosts:
- cert_expires: Oct  5 15:35:38 2026 GMT
  host: vbout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 15:35:38 2026 GMT
  host: api.vbout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vbout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VBOUT, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VBOUT
provider_slug: vbout
slug: vbout-domain-security
source_filename: vbout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vbout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:35:38 2026 GMT\n  hsts: false\n- host: api.vbout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:35:38 2026 GMT\n  hsts: false\ndomains:\n- domain: vbout.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vbout/refs/heads/main/security/vbout-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marketing Automation
- Email Marketing
- Social-Media
- Lead Management
- Landing Pages
- Chatbots
- Contacts
- Campaigns
- Software-as-a-Service
---
