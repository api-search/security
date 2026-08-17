---
api_specs:
- filename: similarweb-account-api-openapi.yml
  format: yaml
  label: SimilarWeb Account API
  slug: similarweb-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-account-api-openapi.yml
- filename: similarweb-app-intelligence-api-openapi.yml
  format: yaml
  label: SimilarWeb App Intelligence API
  slug: similarweb-app-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-app-intelligence-api-openapi.yml
- filename: similarweb-credits-api-openapi.yml
  format: yaml
  label: SimilarWeb Credits API
  slug: similarweb-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-credits-api-openapi.yml
- filename: similarweb-geography-api-openapi.yml
  format: yaml
  label: SimilarWeb Geography API
  slug: similarweb-geography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-geography-api-openapi.yml
- filename: similarweb-integrations-api-openapi.yml
  format: yaml
  label: SimilarWeb Integrations API
  slug: similarweb-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-integrations-api-openapi.yml
- filename: similarweb-keywords-api-openapi.yml
  format: yaml
  label: SimilarWeb Keywords API
  slug: similarweb-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-keywords-api-openapi.yml
- filename: similarweb-lead-enrichment-api-openapi.yml
  format: yaml
  label: SimilarWeb Lead Enrichment API
  slug: similarweb-lead-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-lead-enrichment-api-openapi.yml
- filename: similarweb-rankings-api-openapi.yml
  format: yaml
  label: SimilarWeb Rankings API
  slug: similarweb-rankings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-rankings-api-openapi.yml
- filename: similarweb-reports-api-openapi.yml
  format: yaml
  label: SimilarWeb Reports API
  slug: similarweb-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-reports-api-openapi.yml
- filename: similarweb-similar-sites-api-openapi.yml
  format: yaml
  label: SimilarWeb Similar Sites API
  slug: similarweb-similar-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-similar-sites-api-openapi.yml
- filename: similarweb-traffic-and-engagement-api-openapi.yml
  format: yaml
  label: SimilarWeb Traffic and Engagement API
  slug: similarweb-traffic-and-engagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-traffic-and-engagement-api-openapi.yml
- filename: similarweb-traffic-sources-api-openapi.yml
  format: yaml
  label: SimilarWeb Traffic Sources API
  slug: similarweb-traffic-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-traffic-sources-api-openapi.yml
- filename: similarweb-webhooks-api-openapi.yml
  format: yaml
  label: SimilarWeb Webhooks API
  slug: similarweb-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/openapi/similarweb-webhooks-api-openapi.yml
certifications:
- SOC 2 Type II
- ISO 27001
description: Similarweb operates a dedicated trust center at trustcenter.similarweb.com, linked from its Privacy and Security page. The trust center host itself is behind a Cloudflare interstitial and returned HTTP 403 ("Just a moment...") to an automated fetch, so the certifications below are read from the provider's own Privacy and Security page, which returned 200 and states them in prose.
kind: trust-center
layout: security
name: Similarweb Trust Center
name_suffix: Trust Center
overview: SimilarWeb maintains a public trust center documenting SOC 2 Type II and ISO 27001 compliance.
provider_name: SimilarWeb
provider_slug: similarweb
slug: similarweb-trust-center
source_filename: similarweb-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://trustcenter.similarweb.com/\ndescription: >-\n  Similarweb operates a dedicated trust center at trustcenter.similarweb.com, linked from\n  its Privacy and Security page. The trust center host itself is behind a Cloudflare\n  interstitial and returned HTTP 403 (\"Just a moment...\") to an automated fetch, so the\n  certifications below are read from the provider's own Privacy and Security page, which\n  returned 200 and states them in prose.\n\ncertifications:\n- SOC 2 Type II\n- ISO 27001\n\ncompliance:\n- id: gdpr\n  evidence: https://www.similarweb.com/corp/legal/privacy-policy/\n- id: ccpa\n  evidence: https://www.similarweb.com/corp/legal/privacy-policy/\n\nprogram:\n  described_at: https://www.similarweb.com/corp/privacy-security/\n  practices:\n  - Enterprise information-security policies, technical standards and procedures\n  - Ongoing risk assessments of the corporate network and cloud environments\n\
  \  - Third-party/supplier security review via a dedicated risk-assessment platform\n  - Maintained and regularly tested disaster-recovery and business-continuity plans\n  - Documented security incident response process\n  quote: >-\n    \"We're dedicated to customer data security and hold an independently validated SOC2 and\n    ISO 27001 certification.\"\n\nlegal:\n  privacy_policy: https://www.similarweb.com/corp/legal/privacy-policy/\n  terms: https://www.similarweb.com/corp/legal/terms/\n  contact: legal@similarweb.com\n\ngaps:\n  security_txt: false\n  vulnerability_disclosure_policy: false\n  bug_bounty: false\n  note: >-\n    No /.well-known/security.txt on any host, no responsible-disclosure page, and no\n    HackerOne or Bugcrowd program (both /similarweb handles return 404). A researcher has\n    no published channel for reporting a vulnerability, which is the single clearest gap\n    in an otherwise well-documented security posture. No `Security` pointer is emitted,\n    because\
  \ none is earned.\n\nevidence:\n- {source: https://www.similarweb.com/corp/privacy-security/, http_status: 200, keywords: [SOC2 Type II, ISO 27001, trust center, incident response, risk assessment]}\n- {source: https://trustcenter.similarweb.com/, http_status: 403, note: Cloudflare bot challenge}\n- {source: https://hackerone.com/similarweb, http_status: 404}\n- {source: https://bugcrowd.com/similarweb, http_status: 404}\n- {source: https://www.similarweb.com/.well-known/security.txt, http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/similarweb/refs/heads/main/security/similarweb-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001
tags:
- Digital Intelligence
- Web Analytics
- Traffic Analytics
- Competitive Intelligence
- Keyword Analytics
- Audience Demographics
- App Intelligence
- Market Research
- E-commerce
- SEO
trust_url: https://trustcenter.similarweb.com/
---
