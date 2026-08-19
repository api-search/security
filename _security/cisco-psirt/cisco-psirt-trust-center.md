---
api_specs:
- filename: cisco-psirt-current-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Current Endpoints API
  slug: cisco-psirt-current-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-current-endpoints-api-openapi.yml
- filename: cisco-psirt-obsolete-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Obsolete Endpoints API
  slug: cisco-psirt-obsolete-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-obsolete-endpoints-api-openapi.yml
- filename: cisco-psirt-sunset-endpoints-api-openapi.yml
  format: yaml
  label: Cisco PSIRT openVuln API Sunset Endpoints API
  slug: cisco-psirt-sunset-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/openapi/cisco-psirt-sunset-endpoints-api-openapi.yml
certifications:
- SOC 2
- ISO 27001
- FedRAMP
- BSI C5
- GDPR
description: 'Cisco operates a two-part trust surface: the Trust Center (narrative — trust principles, transparency, responsible-AI framework, vulnerability-disclosure posture) and the Trust Portal (self-service document access — audit reports, penetration tests, security questionnaires, privacy data sheets). Named certifications live on the Portal, not on the Center landing page.'
kind: trust-center
layout: security
name: Cisco Psirt Trust Center
name_suffix: Trust Center
overview: Cisco PSIRT openVuln API maintains a public trust center documenting SOC 2, ISO 27001, FedRAMP, BSI C5, and GDPR compliance.
provider_name: Cisco PSIRT openVuln API
provider_slug: cisco-psirt
slug: cisco-psirt-trust-center
source_filename: cisco-psirt-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nprobe: true\nurl: https://trust.cisco.com/\nresolved_url: https://www.cisco.com/c/en/us/about/trust-center.html\ndescription: >-\n  Cisco operates a two-part trust surface: the Trust Center (narrative — trust\n  principles, transparency, responsible-AI framework, vulnerability-disclosure\n  posture) and the Trust Portal (self-service document access — audit reports,\n  penetration tests, security questionnaires, privacy data sheets). Named\n  certifications live on the Portal, not on the Center landing page.\ntrust_portal: https://trustportal.cisco.com/c/r/ctp/home.html\ncertifications:\n  - SOC 2\n  - ISO 27001\n  - FedRAMP\n  - BSI C5\n  - GDPR\ncertification_note: >-\n  These are the frameworks the Trust Portal names verbatim in its own document\n  categories — \"Audit Reports (SOC, FedRAMP, ISO, C5)\" and Trust Packages\n  containing \"SOC2/ISO 27001 Certification\" and \"Privacy Data Sheet/Maps (GDPR)\".\n  They are CORPORATE\
  \ and PER-PRODUCT attestations obtained through the Portal per\n  Trust Package (AppDynamics, CX Cloud, Webex Meetings, Umbrella, …). The PSIRT\n  openVuln API is NOT itself listed as a Trust Package, so none of these\n  certifications should be read as an attestation scoped to this API.\ndocument_categories:\n  - Audit Reports (SOC, FedRAMP, ISO, C5)\n  - Pen Tests and Security Assessments\n  - Security Questionnaires\n  - Offer Disclosures\n  - Business Continuity / Disaster Recovery\n  - SIG/CAIQ Risk Questionnaire\nrelated:\n  cloud_controls_framework: https://www.cisco.com/c/en/us/about/trust-center/compliance/ccf.html\n  csa_star_registry: https://cloudsecurityalliance.org/star/registry/cisco-systems\nevidence:\n  - source: https://trust.cisco.com/\n    http_status: 200\n    redirects_to: https://www.cisco.com/c/en/us/about/trust-center.html\n    keywords: [trust center, trust portal, transparency, certifications, privacy, compliance]\n    fetched: '2026-08-19'\n  - source: https://trustportal.cisco.com/c/r/ctp/home.html\n\
  \    http_status: 200\n    keywords: [soc2, iso 27001, fedramp, gdpr, c5, compliance]\n    fetched: '2026-08-19'\nnote: >-\n  The automated probe returned trust=none because it only reaches the hosts named\n  in apis.yml. This file is the SEARCHED upgrade against Cisco's real trust hosts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-psirt/refs/heads/main/security/cisco-psirt-trust-center.yml
summary_line: SOC 2, ISO 27001, FedRAMP, BSI C5, GDPR
tags:
- Security
- Vulnerability Management
- Threat Intelligence
- Disclosure
- Compliance
- Networking
trust_url: https://trust.cisco.com/
---
