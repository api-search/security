---
api_specs:
- filename: vessel-platform-openapi.yml
  format: yaml
  label: Vessel Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-platform-openapi.yml
- filename: vessel-crm-openapi.yml
  format: yaml
  label: Vessel CRM Unified API
  slug: crm-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-crm-openapi.yml
- filename: vessel-engagement-openapi.yml
  format: yaml
  label: Vessel Sales Engagement Unified API
  slug: engagement-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-engagement-openapi.yml
- filename: vessel-chat-openapi.yml
  format: yaml
  label: Vessel Chat Unified API
  slug: chat-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-chat-openapi.yml
- filename: vessel-dialer-openapi.yml
  format: yaml
  label: Vessel Dialer Unified API
  slug: dialer-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-dialer-openapi.yml
- filename: vessel-marketing-automation-openapi.yml
  format: yaml
  label: Vessel Marketing Automation Unified API
  slug: marketing-automation-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-marketing-automation-openapi.yml
- filename: vessel-crm-v1-openapi.yml
  format: yaml
  label: Vessel CRM API (v1, legacy)
  slug: crm-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-crm-v1-openapi.yml
- filename: vessel-engagement-v1-openapi.yml
  format: yaml
  label: Vessel Engagement API (v1, legacy)
  slug: engagement-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-engagement-v1-openapi.yml
- filename: vessel-salesforce-actions-openapi.yml
  format: yaml
  label: Vessel Salesforce Actions API
  slug: salesforce-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-salesforce-actions-openapi.yml
- filename: vessel-slack-actions-openapi.yml
  format: yaml
  label: Vessel Slack Actions API
  slug: slack-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-slack-actions-openapi.yml
- filename: vessel-teams-actions-openapi.yml
  format: yaml
  label: Vessel Microsoft Teams Actions API
  slug: teams-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-teams-actions-openapi.yml
- filename: vessel-outreach-actions-openapi.yml
  format: yaml
  label: Vessel Outreach Actions API
  slug: outreach-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-outreach-actions-openapi.yml
- filename: vessel-salesloft-actions-openapi.yml
  format: yaml
  label: Vessel Salesloft Actions API
  slug: salesloft-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-salesloft-actions-openapi.yml
- filename: vessel-apollo-actions-openapi.yml
  format: yaml
  label: Vessel Apollo Actions API
  slug: apollo-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-apollo-actions-openapi.yml
- filename: vessel-aircall-actions-openapi.yml
  format: yaml
  label: Vessel Aircall Actions API
  slug: aircall-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-aircall-actions-openapi.yml
- filename: vessel-dialpad-actions-openapi.yml
  format: yaml
  label: Vessel Dialpad Actions API
  slug: dialpad-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-dialpad-actions-openapi.yml
- filename: vessel-ringcentral-actions-openapi.yml
  format: yaml
  label: Vessel RingCentral Actions API
  slug: ringcentral-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-ringcentral-actions-openapi.yml
- filename: vessel-mailchimp-actions-openapi.yml
  format: yaml
  label: Vessel Mailchimp Actions API
  slug: mailchimp-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-mailchimp-actions-openapi.yml
- filename: vessel-activecampaign-actions-openapi.yml
  format: yaml
  label: Vessel ActiveCampaign Actions API
  slug: activecampaign-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-activecampaign-actions-openapi.yml
- filename: vessel-monday-actions-openapi.yml
  format: yaml
  label: Vessel monday.com Actions API
  slug: monday-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/openapi/vessel-monday-actions-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vessel.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vessel.land
  spf: true
hosts:
- cert_expires: Oct  1 06:58:09 2026 GMT
  host: www.vessel.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 11:24:18 2026 GMT
  host: api.vessel.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.vessel.land
  https: false
kind: domain-security
layout: security
method: probed
name: Vessel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vessel, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vessel
provider_slug: vessel
slug: vessel-domain-security
source_filename: vessel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vessel.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:58:09 2026 GMT\n  hsts: false\n- host: api.vessel.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 11:24:18 2026 GMT\n  hsts: null\n- host: api.vessel.land\n  https: false\ndomains:\n- domain: vessel.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: vessel.land\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vessel/refs/heads/main/security/vessel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CRM
- Chat
- Dialer
- Embedded Integrations
- Go-To-Market
- Integration
- iPaaS
- Marketing Automation
- Sales Engagement
- Unified-API
- Webhook
---
