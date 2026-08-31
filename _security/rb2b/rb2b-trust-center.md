---
certifications:
- SOC 2 Type 2
- CCPA
- GDPR
description: 'RB2B publishes its security posture on its own site and points at a SecurityPal-hosted assurance profile for verification. The trust centre is on the retention.securitypal.com subdomain rather than an rb2b one: RB2B and Retention.com are sibling products of the same company, which is also why www.rb2b.com/apis 301-redirects to retention.com/apis and the database opt-out is operated at app.retention.com/optout. Confirmed by the link being published on RB2B''s own /security page.'
kind: trust-center
layout: security
name: Rb2B Trust Center
name_suffix: Trust Center
overview: RB2B maintains a public trust center documenting SOC 2 Type 2, CCPA, and GDPR compliance.
provider_name: RB2B
provider_slug: rb2b
slug: rb2b-trust-center
source_filename: rb2b-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nprobe: true\nsource: https://www.rb2b.com/security\nurl: https://retention.securitypal.com\ndescription: >-\n  RB2B publishes its security posture on its own site and points at a\n  SecurityPal-hosted assurance profile for verification. The trust centre is on\n  the retention.securitypal.com subdomain rather than an rb2b one: RB2B and\n  Retention.com are sibling products of the same company, which is also why\n  www.rb2b.com/apis 301-redirects to retention.com/apis and the database opt-out\n  is operated at app.retention.com/optout. Confirmed by the link being published\n  on RB2B's own /security page.\ntrust_center:\n  url: https://retention.securitypal.com\n  platform: SecurityPal\n  status: 200\n  probed: '2026-08-12'\ncertifications:\n  - name: SOC 2 Type 2\n    status: certified\n    evidence: '\"RB2B is SOC2 Type 2 Certified and CCPA Compliant\" — https://www.rb2b.com/security'\n  - name: CCPA\n    status: compliant\n    evidence:\
  \ https://www.rb2b.com/security\n  - name: GDPR\n    status: program published\n    evidence: https://www.rb2b.com/gdpr (HTTP 200)\nnot_claimed:\n  - ISO 27001\n  - HIPAA\n  - PCI DSS\n  - FedRAMP\npractices:\n  vulnerability_management: Amazon Inspector for automated, continual vulnerability management\n  monitoring: 24/7\n  data_position: \"We do not repackage or resell your data\"\nprivacy:\n  privacy_policy: https://www.rb2b.com/privacy-policy\n  terms: https://www.rb2b.com/terms-conditions\n  gdpr: https://www.rb2b.com/gdpr\n  compliance: https://www.rb2b.com/compliance\n  privacy_choices: https://www.rb2b.com/your-privacy-choices\n  database_opt_out: https://app.retention.com/optout/\n  compliance_faqs: https://support.rb2b.com/en/articles/15589545-compliance-faqs\n  security_faqs: https://support.rb2b.com/en/articles/8999958-security-faqs\n  vendor_review_policy: https://support.rb2b.com/en/articles/12861177-vendor-reviews-and-security-assessments-policy-for-trials-and-self-serve-plans\n\
  vulnerability_disclosure:\n  program: none\n  evidence: >-\n    No RB2B security.txt, no bug bounty, and no disclosure page. The only\n    /.well-known/security.txt reachable on an rb2b.com host is Intercom's\n    platform document served by the hosted help centre — see\n    well-known/rb2b-well-known.yml. No VulnerabilityDisclosure or Security\n    pointer is emitted for RB2B.\n  security_contact: support@rb2b.com (general support address; no dedicated security address published)\nevidence:\n  - source: https://www.rb2b.com/security\n    keywords: [soc2, soc 2 type 2, ccpa, amazon inspector, 24/7 monitoring]\n  - source: https://retention.securitypal.com\n    keywords: [trust center, assurance profile]\n  - source: https://www.rb2b.com/gdpr\n    keywords: [gdpr]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rb2b/refs/heads/main/security/rb2b-trust-center.yml
summary_line: SOC 2 Type 2, CCPA, GDPR
tags:
- Identity Resolution
- Visitor Identification
- B2B Data
- Lead Generation
- Sales Intelligence
- Marketing
- Data Enrichment
- LinkedIn Enrichment
- Hashed Email
- Mobile Ad ID
- Firmographics
- Webhook
- Pixel
- Adtech
- Identity Graph
- MCP
trust_url: https://retention.securitypal.com
---
