---
api_specs:
- filename: brandwatch-consumer-research-openapi.yml
  format: yaml
  label: Brandwatch Consumer Research API
  slug: consumer-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/openapi/brandwatch-consumer-research-openapi.yml
certifications:
- ISO/IEC 27001:2022
description: ''
kind: trust-center
layout: security
name: Brandwatch Trust Center
name_suffix: Trust Center
overview: Brandwatch maintains a public trust center documenting ISO/IEC 27001:2022 compliance.
provider_name: Brandwatch
provider_slug: brandwatch
slug: brandwatch-trust-center
source_filename: brandwatch-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://www.brandwatch.com/legal/information-security/\ntitle: The Brandwatch Security Programme\nformat: single long-form page\nformat_note: >-\n  Not a hosted trust portal — trust.brandwatch.com does not resolve (DNS\n  NXDOMAIN) and there is no Vanta/Drata/SafeBase surface. What Brandwatch\n  publishes is one twelve-section security programme page under /legal/. It is\n  unusually detailed for a page of that kind: named hosting providers, named\n  data-centre locations, retention windows, password policy and encryption\n  specifics are all stated in the open.\ncertifications:\n  - name: ISO/IEC 27001:2022\n    scope: all Brandwatch products\n    status: certified\n    audit_cadence: at least annually, third party\n    certificate_availability: on request via a Brandwatch contact\n    evidence: >-\n      \"All Brandwatch products are ISO 27001:2022 certified ... We engage a\n      third party to audit our adherence\
  \ to these standards at least annually.\n      Our current ISO 27001 certificate is available upon request.\"\nnot_claimed:\n  - SOC 2\n  - PCI DSS\n  - HIPAA\n  - FedRAMP\n  - CSA STAR\n  - ISO 27017\n  - ISO 27018\nnot_claimed_note: >-\n  None of these appear anywhere on the Brandwatch security or legal pages.\n  Recorded as an explicit absence so a later pass does not assume them.\nsections:\n  - Programme Overview\n  - Data Centres and Third Party Hosting\n  - Access Control and Data Protection\n  - Device and Network Security\n  - Business Continuity, Disaster Recovery, and SLAs\n  - Security in Development\n  - Vendor and Contractor Security\n  - Data Breach Notification\n  - Privacy, legal, and regulatory Compliance\n  - ISO/IEC 27001 Compliance\n  - Vulnerability Disclosure\n  - Feedback\npublished_facts:\n  hosting:\n    - provider: AWS\n      use: Consumer Research raw data ingestion, indexing, analysis and storage\n      region: US\n    - provider: Google Cloud Platform\n  \
  \    use: Consumer Research frontend applications and Vizia components\n      region: Europe\n    - provider: Virtus DC (Hayes, UK)\n      use: analysis results and customer metadata, colocation\n      region: UK\n    - provider: AWS and GCP\n      use: Social Media Management products\n      region: EU (Listening infrastructure in US and UK, public data only)\n    - provider: Heroku and AWS\n      use: Influence (formerly Paladin)\n      region: US\n    - provider: Linode, Aiven\n      use: supplementary\n  sub_processors: https://www.brandwatch.com/legal/sub-processors/\n  sub_processor_subscriptions: https://www.brandwatch.com/legal/sub-processors/#subscribe-to-sub-processor-changes\n  encryption_in_transit: TLS 1.2 and 1.3, TLS 1.2 by default\n  encryption_at_rest: SSE-S3 for uploaded data and backups; AES-256 for physical backup tapes\n  data_retention_after_termination: 30 days maximum, then automated deletion or anonymization\n  sso:\n    consumer_research: SAML 2.0 and Google Authentication,\
  \ premium feature; no SCIM provisioning\n    social_media_management: SAML, OpenID Connect, Google/Facebook/Twitter/LinkedIn, 2FA — included at no cost\n  password_policy: bcrypt hashed and salted, 8 char minimum with numeric and special, optional 90-day expiry, lockout after 10 failures\n  security_training: OWASP Top 10 refresher training for staff\nprivacy:\n  user_privacy_policy: https://www.brandwatch.com/legal/user-privacy-policy/\n  author_privacy_policy: https://www.brandwatch.com/legal/author-privacy-policy/\n  data_subject_access_request: https://www.brandwatch.com/legal/data-subject-access-request/\n  contact: privacy@brandwatch.com\n  note: >-\n    Brandwatch publishes a separate Author Privacy Policy covering the social\n    media authors whose public posts it indexes — the data subjects who are not\n    its customers. That is a distinctive and relevant artifact for a social\n    listening platform.\nlegal:\n  hub: https://www.brandwatch.com/legal/\n  terms: https://www.cision.com/legal/msa/\n\
  \  terms_note: >-\n    Brandwatch's Terms & Conditions link resolves to the Master Services\n    Agreement of its parent, Cision Group Ltd. Brandwatch has been part of\n    Cision since 2021 and the site footer identifies the operating entity as\n    Cision Group Ltd, company number 03898053.\n  modern_slavery_statement: https://www.cision.com/content/dam/cision-revamp/cision-optimized/legal/2025%20Modern%20Slavery%20Statement.pdf\nevidence:\n  - source: https://www.brandwatch.com/legal/information-security/\n    status: 200\n    keywords:\n      - ISO 27001:2022\n      - security programme\n      - vulnerability disclosure\n      - data breach notification\n      - sub processors\n  - source: https://trust.brandwatch.com\n    status: 000\n    finding: DNS does not resolve — no hosted trust portal\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/security/brandwatch-trust-center.yml
summary_line: ISO/IEC 27001:2022
tags:
- Analytics
- Social-Media
- Social Media Monitoring
- Consumer Intelligence
- Brand Management
- Sentiment Analysis
trust_url: https://www.brandwatch.com/legal/information-security/
---
