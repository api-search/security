---
api_specs:
- filename: fullenrich-contact-enrichment-api-openapi.yml
  format: yaml
  label: FullEnrich Contact Enrichment API
  slug: fullenrich-contact-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-contact-enrichment-api-openapi.yml
- filename: fullenrich-reverse-email-lookup-api-openapi.yml
  format: yaml
  label: FullEnrich Reverse Email Lookup API
  slug: fullenrich-reverse-email-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-reverse-email-lookup-api-openapi.yml
- filename: fullenrich-search-api-openapi.yml
  format: yaml
  label: FullEnrich Search API
  slug: fullenrich-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-search-api-openapi.yml
- filename: fullenrich-lookup-api-openapi.yml
  format: yaml
  label: FullEnrich Lookup API
  slug: fullenrich-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-lookup-api-openapi.yml
- filename: fullenrich-account-api-openapi.yml
  format: yaml
  label: FullEnrich Account API
  slug: fullenrich-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-account-api-openapi.yml
certifications:
- SOC 2 Type II
- GDPR
- CCPA
description: FullEnrich's Privacy & Legal Center doubles as its trust center, publishing compliance badges, an Article 32 security-measures summary, a public DPA, a sub-processor list, and a request path to the SOC 2 Type II report through a hosted trust portal.
kind: trust-center
layout: security
name: Fullenrich Trust Center
name_suffix: Trust Center
overview: FullEnrich maintains a public trust center documenting SOC 2 Type II, GDPR, and CCPA compliance.
provider_name: FullEnrich
provider_slug: fullenrich
slug: fullenrich-trust-center
source_filename: fullenrich-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nprobe: false\nprobe_note: >-\n  DO NOT let probe-security-programs.py overwrite this file. Its keyword matcher\n  credits FullEnrich with ISO 27001 because the string appears once on the trust\n  page — describing DigitalOcean, the hosting sub-processor. This file is the\n  human-verified reading and is the stronger artifact.\nsource: https://fullenrich.com/trust\nurl: https://fullenrich.com/trust\ndescription: >-\n  FullEnrich's Privacy & Legal Center doubles as its trust center, publishing\n  compliance badges, an Article 32 security-measures summary, a public DPA, a\n  sub-processor list, and a request path to the SOC 2 Type II report through a\n  hosted trust portal.\n\ncertifications:\n- SOC 2 Type II\n- GDPR\n- CCPA\n\ncorrections:\n- previously_recorded: ISO 27001\n  status: removed\n  reason: >-\n    MISATTRIBUTION. An automated keyword pass matched \"ISO 27001\" on this page and\n    credited it to FullEnrich. The only occurrence\
  \ describes the hosting\n    sub-processor: \"data hosting provider (DigitalOcean) is compliant with SOC 2\n    and ISO 27001 standards\". FullEnrich holds no ISO 27001 certification of its\n    own and claims none anywhere on the site.\n  verified: '2026-08-14'\n  verification_method: >-\n    Fetched https://fullenrich.com/trust and inspected every occurrence of\n    \"iso 27001\" in context (1 occurrence, sub-processor clause).\n\ndocuments_published:\n- name: Data Processing Agreement (DPA)\n  public: true\n  detail: Publicly available, covers GDPR Article 28 obligations, signable as part of the commercial relationship.\n- name: Terms and Conditions of Use and Sale\n  public: true\n  url: https://fullenrich.com/tos\n  last_updated: '2026-08-11'\n- name: Privacy Policy\n  public: true\n  url: https://fullenrich.com/privacy-policy\n- name: List of Sub-processors\n  public: true\n- name: Cookie Policy\n  public: true\n- name: Do Not Sell My Information\n  public: true\n- name: Security\
  \ Documentation\n  public: false\n  detail: Available on request through the trust center.\n- name: SOC 2 Type II Compliance Report\n  public: false\n  detail: Access requested through the hosted trust portal.\n\nhosted_trust_portal:\n  url: https://trust.delve.co/fullenrich\n  vendor: Delve\n  probe_status: 429\n  probe_note: >-\n    The portal answered with a Vercel Security Checkpoint bot challenge rather than\n    the page. We do not evade challenges, so its contents were not read; its\n    existence and purpose are taken from the link and description on\n    https://fullenrich.com/trust and https://fullenrich.com/pricing.md.\n\nsecurity_measures_published:\n  standard: GDPR Article 32\n  measures:\n  - Regular testing, assessment and evaluation of technical and organizational measures\n  - 'Identification and authorization: session cookies (JWT) signed with HMAC-SHA256, plus RBAC'\n  - Data at rest protected by AES encryption\n  - Event logging retained 1 year, encrypted at rest\n\
  \  - Data minimization\n  - Limited data retention (enrichment data kept 3 months)\n  - Contractual measures flowed down to sub-processors\n  pentesting: Regular penetration tests\n\ndata_handling:\n  hosting_provider: DigitalOcean\n  hosting_region: European Union\n  hosting_provider_certifications:\n  - SOC 2\n  - ISO 27001\n  hosting_provider_note: >-\n    These belong to DigitalOcean, not FullEnrich. Recorded here so the distinction\n    stays explicit and the misattribution does not recur.\n  international_transfers: Standard Contractual Clauses\n  processing_role: Processor for Waterfall Enrichment\n  database_claim: >-\n    FullEnrich states the Waterfall Enrichment service does not rely on a database\n    and does not create one from customer results — enrichment is real-time.\n  breach_process: >-\n    When acting as controller, FullEnrich states it will directly inform data\n    subjects where necessary.\n\nevidence:\n- source: https://fullenrich.com/trust\n  http_status: 200\n\
  \  keywords: [soc 2 type 2 certified, gdpr compliant, ccpa compliant, trust center, dpa, sub-processors, pentest]\n- source: https://fullenrich.com/pricing.md\n  http_status: 200\n  keywords: [soc 2 type ii, gdpr, ccpa]\n- source: https://trust.delve.co/fullenrich\n  http_status: 429\n  note: bot challenge, not read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/security/fullenrich-trust-center.yml
summary_line: SOC 2 Type II, GDPR, CCPA
tags:
- B2B Data
- Contact Enrichment
- Email Finder
- Phone Finder
- Waterfall Enrichment
- Sales Intelligence
- People Search
- Company Search
- Reverse Email Lookup
- Agent Ready
trust_url: https://fullenrich.com/trust
---
