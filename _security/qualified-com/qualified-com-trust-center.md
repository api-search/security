---
api_specs:
- filename: qualified-com-bot-conversations-api-openapi.yml
  format: yaml
  label: Qualified Bot Conversations API
  slug: qualified-com-bot-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-bot-conversations-api-openapi.yml
- filename: qualified-com-bulk-api-openapi.yml
  format: yaml
  label: Qualified Bulk API
  slug: qualified-com-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-bulk-api-openapi.yml
- filename: qualified-com-cancel-meeting-api-openapi.yml
  format: yaml
  label: Qualified Cancel Meeting API
  slug: qualified-com-cancel-meeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-cancel-meeting-api-openapi.yml
- filename: qualified-com-companies-api-openapi.yml
  format: yaml
  label: Qualified Companies API
  slug: qualified-com-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-companies-api-openapi.yml
- filename: qualified-com-conversations-api-openapi.yml
  format: yaml
  label: Qualified Conversations API
  slug: qualified-com-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-conversations-api-openapi.yml
- filename: qualified-com-emails-api-openapi.yml
  format: yaml
  label: Qualified Emails API
  slug: qualified-com-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-emails-api-openapi.yml
- filename: qualified-com-gdpr-api-openapi.yml
  format: yaml
  label: Qualified GDPR API
  slug: qualified-com-gdpr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-gdpr-api-openapi.yml
- filename: qualified-com-leads-api-openapi.yml
  format: yaml
  label: Qualified Leads API
  slug: qualified-com-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-leads-api-openapi.yml
- filename: qualified-com-meetings-api-openapi.yml
  format: yaml
  label: Qualified Meetings API
  slug: qualified-com-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-meetings-api-openapi.yml
- filename: qualified-com-messages-api-openapi.yml
  format: yaml
  label: Qualified Messages API
  slug: qualified-com-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-messages-api-openapi.yml
- filename: qualified-com-rep-conversations-api-openapi.yml
  format: yaml
  label: Qualified Rep Conversations API
  slug: qualified-com-rep-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-rep-conversations-api-openapi.yml
- filename: qualified-com-sessions-api-openapi.yml
  format: yaml
  label: Qualified Sessions API
  slug: qualified-com-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/openapi/qualified-com-sessions-api-openapi.yml
certifications:
- SOC 2 Type II
- EU-US Privacy Shield
description: ''
kind: trust-center
layout: security
name: Qualified Com Trust Center
name_suffix: Trust Center
overview: Qualified maintains a public trust center documenting SOC 2 Type II and EU-US Privacy Shield compliance.
provider_name: Qualified
provider_slug: qualified-com
slug: qualified-com-trust-center
source_filename: qualified-com-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://www.qualified.com/trust\ntrust_center_url: https://www.qualified.com/trust\nalternate_url: https://trust.qualified.com/\nnote: >-\n  trust.qualified.com resolves and returns HTTP 200 but serves a 5.6KB client-rendered\n  shell with no readable content; https://www.qualified.com/trust is the substantive page\n  and is what is recorded here. Qualified also operates a gated Trust Center from which\n  full policies, the SOC 2 Type II report and the penetration-test summary are released to\n  customers and prospects under NDA.\ncertifications:\n- name: SOC 2 Type II\n  status: audited annually\n  public_report: false\n  access: Contact your Qualified Representative to request the current report.\n- name: EU-US Privacy Shield\n  status: historical\n  note: >-\n    Qualified was previously certified; the framework was invalidated by the CJEU in\n    Schrems II (16 July 2020) and Qualified now relies on Standard Contractual\
  \ Clauses.\ncompliance_programs:\n- name: GDPR\n  url: https://www.qualified.com/legal/gdpr\n  contact: privacy@qualified.com\n- name: CCPA\n  role: Service Provider\n  note: Qualified states it does not sell customer personal information. California Annex in the DPA.\n- name: Standard Contractual Clauses\n  note: Used for transfers of personal data into the U.S., covering Qualified and all sub-processors.\n- name: Data Processing Agreement\n  url: https://www.qualified.com/legal/data-processing-addendum\n- name: Sub-processor list\n  url: https://www.qualified.com/legal/subprocessors\nsecurity_program:\n  hosting: Amazon Web Services\n  access_control: least privilege, regular access reviews, SSO and MFA\n  encryption: encryption of data in motion over public networks\n  ddos_mitigation: true\n  intrusion_detection: IDS + SIEM on the corporate network, plus AWS controls in production\n  penetration_testing:\n    frequency: annually at minimum\n    type: black box\n    conducted_by: independent\
  \ third-party agency\n    method: >-\n      Qualified provides the agency an isolated clone of Qualified.com and a high-level\n      application architecture diagram. Exploited vulnerabilities are tracked, assigned for\n      remediation, and retested.\n    summary_availability: A summary of the most recent test is available in the gated Trust Center.\n  business_continuity:\n    bcp_tested: annually\n    owner: CTO\n    postmortem_required: true\n  ai_governance:\n    framework: Qualified AI Trust Framework\n    principles: [Transparency, Fairness, Accountability, Privacy]\n    note: >-\n      Named governance body reviews and approves all AI projects. Relevant because the\n      product is an autonomous AI agent acting on customer buyers.\npublished_policies:\n- Acceptable Use Policy\n- Asset Management Policy\n- Backup Policy\n- Change Management & SDLC Policy\n- Code of Conduct\n- Cryptography Policy\n- Data Management Policy\n- Disaster Recovery Plan\n- Generative AI in the Workplace\
  \ Policy\n- Incident Response Plan\n- Passwords Policy\n- Physical Security Policy\n- Responsible Disclosure Policy\n- Risk Assessment Policy\n- System Access Control Policy\n- Vendor Management Policy\n- Vulnerability Management Policy\npolicy_access: >-\n  Policy NAMES are public on the trust page; the policy TEXT is released to prospective and\n  existing customers under a signed NDA through the gated Trust Center.\ncontacts:\n  security: security@qualified.com\n  privacy: privacy@qualified.com\nstatus_page: https://status.qualified.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualified-com/refs/heads/main/security/qualified-com-trust-center.yml
summary_line: SOC 2 Type II, EU-US Privacy Shield
tags:
- Company
- Conversational Marketing
- Sales
- Marketing
- Artificial Intelligence
- AI Agents
- Lead Generation
- Customer Engagement
- Salesforce
- Analytics
trust_url: ''
---
