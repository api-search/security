---
api_specs:
- filename: clay-com-me-api-openapi.yml
  format: yaml
  label: Clay Me API
  slug: clay-com-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay-com/refs/heads/main/openapi/clay-com-me-api-openapi.yml
- filename: clay-com-routines-api-openapi.yml
  format: yaml
  label: Clay Routines API
  slug: clay-com-routines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay-com/refs/heads/main/openapi/clay-com-routines-api-openapi.yml
- filename: clay-com-search-api-openapi.yml
  format: yaml
  label: Clay Search API
  slug: clay-com-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay-com/refs/heads/main/openapi/clay-com-search-api-openapi.yml
- filename: clay-com-tables-api-openapi.yml
  format: yaml
  label: Clay Tables API
  slug: clay-com-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clay-com/refs/heads/main/openapi/clay-com-tables-api-openapi.yml
certifications:
- SOC 2 Type II
- ISO 27001
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Clay Com Trust Center
name_suffix: Trust Center
overview: Clay maintains a public trust center documenting SOC 2 Type II, ISO 27001, GDPR, and CCPA compliance.
provider_name: Clay
provider_slug: clay-com
slug: clay-com-trust-center
source_filename: clay-com-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: true\nurl: https://trust.clay.com\nplatform: Vanta\ncertifications:\n- name: SOC 2 Type II\n  status: certified\n  first_completed: '2024-09-09'\n  evidence:\n  - url: https://www.clay.com/enterprise\n    quote: 'We are SOC 2 Type II compliant. Request our SOC 2 in our Trust Center.'\n  - url: https://www.clay.com/blog/clay-is-soc-2-type-2-compliant\n    quote: 'Clay has completed our SOC 2 Type 2 audit'\n- name: ISO 27001\n  status: named\n  evidence:\n  - url: https://www.clay.com/enterprise\n    note: Named in Clay's own enterprise security section.\n- name: GDPR\n  status: named\n  evidence:\n  - url: https://www.clay.com/enterprise\n    quote: 'Go to market anywhere in the world — let us handle compliance with local laws.'\n- name: CCPA\n  status: named\n  evidence:\n  - url: https://www.clay.com/enterprise\n    quote: 'Support your customer base with opt out and DNC support.'\nreport_access: on request via the trust center\n\
  privacy_center: https://privacy.clay.com\nevidence:\n- source: https://www.clay.com/.well-known/security.txt\n  kind: security.txt\n  http_status: 200\n  note: 'Names https://trust.clay.com as both a Contact and the Policy URL — the trust center is the published disclosure destination.'\n- source: https://trust.clay.com\n  kind: trust-center\n  http_status: 200\n  keywords: [vanta]\n- source: https://www.clay.com/enterprise\n  kind: enterprise-security-page\n  http_status: 200\n  keywords: [soc 2 type ii, iso 27001, gdpr, ccpa]\ncaveat: >-\n  trust.clay.com returns HTTP 200 but is a fully client-rendered Vanta trust page — the\n  served HTML contains only the Vanta loader, so the certification list could NOT be read\n  out of the response body. The certifications above are therefore recorded from pages\n  Clay renders server-side (its enterprise page and its own announcement post), not from\n  the trust center itself. The trust center's existence and its role as the security.txt\n  Policy\
  \ target are directly verified; its contents are not machine-readable. That is a\n  provider-side gap: an agent evaluating Clay's compliance posture cannot read it.\nsubprocessors:\n  published: true\n  location: https://trust.clay.com\n  note: Clay states a full list of AI subprocessors is available in the trust center.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clay-com/refs/heads/main/security/clay-com-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, GDPR, CCPA
tags:
- Prospecting
- GTM
- Sales
- Enrichment
- Automation
- Artificial Intelligence
- Webhook
trust_url: https://trust.clay.com
---
