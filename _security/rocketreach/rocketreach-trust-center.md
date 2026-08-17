---
api_specs:
- filename: rocketreach-account-api-openapi.yml
  format: yaml
  label: RocketReach Account API
  slug: rocketreach-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-account-api-openapi.yml
- filename: rocketreach-company-data-api-api-openapi.yml
  format: yaml
  label: RocketReach Company Data API API
  slug: rocketreach-company-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-company-data-api-api-openapi.yml
- filename: rocketreach-people-data-api-api-openapi.yml
  format: yaml
  label: RocketReach People Data API API
  slug: rocketreach-people-data-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-people-data-api-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Rocketreach Trust Center
name_suffix: Trust Center
overview: RocketReach maintains a public trust center covering its security and compliance posture.
provider_name: RocketReach
provider_slug: rocketreach
slug: rocketreach-trust-center
source_filename: rocketreach-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: DNS CNAME + live HTTP probe of https://trust.rocketreach.co\ntrust_center:\n  url: https://trust.rocketreach.co\n  exists: true\n  platform: Drata Trust Center\n  platform_evidence: trust.rocketreach.co CNAMEs to trust.cname.drata.com\n  readable: false\n  http_status: 403\n  blocked_by: Cloudflare managed bot challenge (\"Just a moment...\", cf_chl interstitial, JavaScript required)\ncertifications: []\ncertifications_note: >-\n  NO certification is asserted here. RocketReach runs a Drata-hosted trust center on its own subdomain — that\n  much is proven by the CNAME and by the host answering — but the page itself is behind a Cloudflare\n  challenge that a non-browser client cannot pass, so the named certifications (SOC 2, ISO 27001 or otherwise)\n  could not be read and must not be inferred from the platform choice. Recording the surface without the\n  contents is the honest result. A follow-up with the provider, or a browser-rendered\
  \ fetch, would close this.\nrelated_pages:\n- url: https://rocketreach.co/gdpr\n  status: 200\n  kind: GDPR policy statement (not an attestation)\n- url: https://rocketreach.co/ccpa\n  status: 200\n  kind: CCPA policy statement (not an attestation)\n- url: https://rocketreach.co/privacy\n  status: 200\n  kind: Privacy policy\n- url: https://rocketreach.co/terms\n  status: 200\n  kind: Terms of use\n- url: https://rocketreach.co/security\n  status: 404\n  kind: >-\n    Stale. A TrustCenter pointer in this repo previously named this URL; it 404s. Corrected to\n    https://trust.rocketreach.co in this pass.\nx-evidence:\n- url: https://trust.rocketreach.co\n  http_status: 403\n  fetched: '2026-08-13'\n- url: https://rocketreach.co/security\n  http_status: 404\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/security/rocketreach-trust-center.yml
summary_line: trust center published
tags:
- B2B
- Contact Data
- Email Lookup
- Phone Lookup
- Sales Intelligence
- Lead Generation
- People Search
- Company Search
- Data Enrichment
- Prospecting
- Recruiting
- Webhooks
trust_url: ''
---
