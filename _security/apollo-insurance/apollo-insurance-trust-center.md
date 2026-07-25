---
api_specs:
- filename: apollo-insurance-affiliates.yml
  format: yaml
  label: APOLLO Affiliates API
  slug: apollo-affiliates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/openapi/apollo-insurance-affiliates.yml
- filename: apollo-insurance-affiliates-legacy.yml
  format: yaml
  label: APOLLO Public API - Affiliates
  slug: apollo-public-api-affiliates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/openapi/apollo-insurance-affiliates-legacy.yml
- filename: apollo-insurance-covertrack.yml
  format: yaml
  label: APOLLO CoverTrack API
  slug: apollo-covertrack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/openapi/apollo-insurance-covertrack.yml
certifications:
- SOC 2
- ISO 27001
- PCI DSS
description: ''
kind: trust-center
layout: security
name: Apollo Insurance Trust Center
name_suffix: Trust Center
overview: APOLLO Insurance maintains a public trust center documenting SOC 2, ISO 27001, and PCI DSS compliance.
provider_name: APOLLO Insurance
provider_slug: apollo-insurance
slug: apollo-insurance-trust-center
source_filename: apollo-insurance-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nprobe: true\nsource: https://apollocover.com/security\nurl: https://apollocover.com/security\ntitle: Security at APOLLO\ntype: security-posture-page\nnote: >-\n  This is a published security posture page, not a trust portal. There is no trust.apollocover.com,\n  no document request flow, no audit report, no certificate and no subprocessor list. It is\n  detailed and specific — unusually so for a Canadian broker — but every named certification is\n  INHERITED from an infrastructure or payment vendor. APOLLO does not claim a SOC 2, ISO 27001 or\n  PCI DSS certification of its own.\n\ncertifications:\n- SOC 2\n- ISO 27001\n- PCI DSS\n\ncertifications_detail:\n- name: SOC 2 Type 2\n  held_by: AWS data centres, and Stripe\n  apollo_held: false\n  quote: >-\n    \"The data centers used for storing your content and allowing it to be delivered to your users\n    are also certified for compliance with the SOC 2 Type 2 standard.\"\n- name: ISO\
  \ 27001\n  held_by: AWS\n  apollo_held: false\n  quote: >-\n    \"Physical security to our servers and to your data is managed by AWS security certifications\"\n    (linking to https://aws.amazon.com/compliance/iso-27001-faqs/)\n- name: PCI DSS\n  held_by: Stripe\n  apollo_held: false\n  quote: >-\n    \"APOLLO uses Stripe to process credit card payments, which means that no credit card\n    information or related payment information is stored on our servers. Stripe enforces\n    stringent PCI DSS (Payment Card Industry) compliance criteria...\"\n\napollo_operated_controls:\n  encryption:\n    at_rest: AES-256 in AWS S3, DynamoDB and EBS; keys in AWS KMS\n    in_transit: HTTPS/TLS v1.2 minimum, including to the CDN\n  testing: annual third-party penetration tests of infrastructure, web applications and APIs\n  vulnerability_management: internal severity classification with an internal SLA for fixes, post-mortems where warranted\n  sdlc: >-\n    Bitbucket pull-request peer review, pair\
  \ programming, automatic static code analysis and\n    dependency scanning (SonarCloud) in CI, separate QA AWS account with no production data,\n    security-by-design embedded in the product organisation\n  monitoring: AWS GuardDuty, DataDome (bot/fraud/DDoS), third-party 24/7 SOC, CloudTrail across all environments, OpsGenie escalation\n  network: AWS security groups, Web Application Firewall, AWS Shield\n  access: role- and permission-based access to customer data, all actions recorded and audited; MFA enforced across AWS and Bitbucket\n  resilience: multi-region replication, versioned S3 buckets, point-in-time recovery to 35 days\n  data_retention: documented Data Retention and Data Classification policies; application logs retained 365 days minimum\n  incident_response: >-\n    documented incident response plan covering notification and cooperation with customers, data\n    protection authorities and law enforcement; affected customers notified without undue delay\n  people: security\
  \ and privacy training for employees and contractors, confidentiality clauses in standard contracts\n  vendor_management: risk assessment of every SaaS/tool; contractual privacy and security commitments required of third parties\n  end_user_controls: two-factor authentication via email; minimum 8-character password policy with complexity requirement\n\ngaps:\n  vulnerability_disclosure: >-\n    No coordinated vulnerability disclosure channel. The page describes internal vulnerability\n    management but publishes no security contact address, no responsible-disclosure policy, no\n    safe-harbour statement and no bug bounty. There is no /.well-known/security.txt on any host.\n    A researcher who found a flaw would have to use the general contact form.\n  audit_reports: none offered, and no request mechanism\n  subprocessors: no subprocessor list published\n  own_certifications: none — every named certification belongs to AWS or Stripe\n  status_page: none\n  privacy_regime: >-\n    PIPEDA\
  \ and provincial privacy law apply, and a public privacy policy exists\n    (https://apollocover.com/privacy-policy), but the security page makes no explicit PIPEDA,\n    Law 25 or GDPR statement.\n\nevidence:\n- source: https://apollocover.com/security\n  kind: security-posture-page\n  keywords:\n  - soc 2 type 2\n  - iso 27001\n  - pci dss\n  - penetration test\n  - vulnerability management\n  - incident response\n  - encryption at rest\n  - aws kms\n  - datadome\n  - guardduty\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-insurance/refs/heads/main/security/apollo-insurance-trust-center.yml
summary_line: SOC 2, ISO 27001, PCI DSS
tags:
- Insurance
- Canada
- Insurtech
- Broker
- Embedded Insurance
- Property and Casualty
- Tenant Insurance
- Quoting
- Distribution
- Compliance
trust_url: https://apollocover.com/security
---
