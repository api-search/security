---
api_specs:
- filename: asknicely-contacts-api-openapi.yml
  format: yaml
  label: AskNicely Contacts API
  slug: asknicely-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-contacts-api-openapi.yml
- filename: asknicely-in-app-surveys-api-openapi.yml
  format: yaml
  label: AskNicely In-App Surveys API
  slug: asknicely-in-app-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-in-app-surveys-api-openapi.yml
- filename: asknicely-responses-api-openapi.yml
  format: yaml
  label: AskNicely Responses API
  slug: asknicely-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-responses-api-openapi.yml
- filename: asknicely-statistics-api-openapi.yml
  format: yaml
  label: AskNicely Statistics API
  slug: asknicely-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-statistics-api-openapi.yml
- filename: asknicely-surveys-api-openapi.yml
  format: yaml
  label: AskNicely Surveys API
  slug: asknicely-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-surveys-api-openapi.yml
certifications:
- SOC 2
- ISO 27001
- PCI DSS
- GDPR
- CSA STAR (CAIQ)
- New Zealand Privacy Act
description: AskNicely publishes a single public security page rather than a dedicated trust centre or trust portal. It names the compliance programme AskNicely itself holds (SOC 2, annual penetration testing, CSA CAIQ registry entry) separately from the certifications inherited from its AWS hosting (ISO 27001, PCI).
kind: trust-center
layout: security
name: Asknicely Trust Center
name_suffix: Trust Center
overview: AskNicely maintains a public trust center documenting SOC 2, ISO 27001, PCI DSS, GDPR, CSA STAR (CAIQ), and New Zealand Privacy Act compliance.
provider_name: AskNicely
provider_slug: asknicely
slug: asknicely-trust-center
source_filename: asknicely-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nprobe: true\nsource: https://www.asknicely.com/security\nurl: https://www.asknicely.com/security\ndescription: >-\n  AskNicely publishes a single public security page rather than a dedicated trust centre or trust portal.\n  It names the compliance programme AskNicely itself holds (SOC 2, annual penetration testing, CSA CAIQ\n  registry entry) separately from the certifications inherited from its AWS hosting (ISO 27001, PCI).\ncertifications:\n- SOC 2\n- ISO 27001\n- PCI DSS\n- GDPR\n- CSA STAR (CAIQ)\n- New Zealand Privacy Act\ncertification_detail:\n- name: SOC 2\n  held_by: AskNicely\n  detail: AskNicely states it is SOC-2 compliant and maintains compliance through an annual independent audit.\n- name: ISO 27001\n  held_by: AWS (hosting provider)\n  detail: Inherited from the AWS datacenters AskNicely runs on; not an AskNicely certification.\n- name: PCI DSS\n  held_by: AWS (hosting provider)\n  detail: Inherited from the AWS datacenters\
  \ AskNicely runs on; not an AskNicely certification.\n- name: CSA STAR (CAIQ)\n  held_by: AskNicely\n  detail: AskNicely maintains a public entry in the Cloud Security Alliance registry.\n- name: GDPR\n  held_by: AskNicely\n  detail: GDPR compliance documented; a data processing addendum is available.\n- name: New Zealand Privacy Act\n  held_by: AskNicely\n  detail: Primary jurisdiction for AskNicely, headquartered in Auckland, New Zealand.\npractices:\n  penetration_testing: Annual penetration testing of web and mobile applications.\n  third_party_scans: Third-party security scans and audits conducted regularly.\n  encryption_in_transit: TLS with forward secrecy; HSTS enabled; states an \"A\" rating on Qualys SSL Labs.\n  encryption_at_rest: RDS encryption for the Australia and Europe regions and new US plans.\n  backups: Automated backups with 14-day point-in-time recovery.\n  monitoring: Amazon Inspector (vulnerability scanning), GuardDuty (intrusion detection), Macie (data leak scanning).\n\
  \  hosting_regions: [AWS Oregon (US), AWS Sydney (AU), AWS Frankfurt (EU)]\ngaps:\n- No published vulnerability-disclosure or responsible-disclosure policy.\n- No bug bounty programme.\n- No /.well-known/security.txt on any AskNicely host.\n- No dedicated security contact address published on the security page.\nevidence:\n- source: https://www.asknicely.com/security\n  http_status: 200\n  keywords: [soc 2, iso 27001, pci, gdpr, cloud security alliance, penetration testing]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/security/asknicely-trust-center.yml
summary_line: SOC 2, ISO 27001, PCI DSS, GDPR, CSA STAR (CAIQ), New Zealand Privacy Act
tags:
- Company
- Customer Experience
- Net Promoter Score
- Surveys
- Feedback
- Reputation Management
- Software-as-a-Service
- Customer Success
- Reviews
- SMS
trust_url: https://www.asknicely.com/security
---
