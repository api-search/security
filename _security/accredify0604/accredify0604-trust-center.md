---
api_specs:
- filename: accredify0604-nexus-auth-openapi.yaml
  format: yaml
  label: Accredify Nexus API
  slug: accredify0604-nexus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredify0604/refs/heads/main/openapi/accredify0604-nexus-auth-openapi.yaml
- filename: accredify0604-dashboard-v1-openapi.yaml
  format: yaml
  label: Accredify Dashboard API
  slug: accredify0604-dashboard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accredify0604/refs/heads/main/openapi/accredify0604-dashboard-v1-openapi.yaml
certification_count: 6
certifications:
- ISO/IEC 27001:2022
- ISO/IEC 27017:2015
- ISO/IEC 27018:2019
- CSA STAR CAIQ
- ISO 22301
- IMDA Data Protection Trustmark
description: ''
kind: trust-center
layout: security
name: Accredify0604 Trust Center
name_suffix: Trust Center
overview: Accredify maintains a public trust center documenting ISO/IEC 27001:2022, ISO/IEC 27017:2015, ISO/IEC 27018:2019, CSA STAR CAIQ, ISO 22301, and IMDA Data Protection Trustmark compliance.
provider_name: Accredify
provider_slug: accredify0604
slug: accredify0604-trust-center
source_filename: accredify0604-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://www.accredify.io/security, https://www.accredify.io/multi-standard-flexibility,\n  https://www.accredify.io/data-protection-notice\nurl: https://www.accredify.io/security\nstatus: 200\nnote: >-\n  Accredify publishes a full security posture page rather than a hosted trust-center portal.\n  It names downloadable certificates and describes infrastructure, network, application and\n  continuity controls in specific terms. There is no automated evidence portal, no NDA-gated\n  document room, and no vulnerability disclosure programme or security contact anywhere on\n  the surface.\ncertifications:\n- name: ISO/IEC 27001:2022\n  evidence: https://www.accredify.io/security — \"Download ISO 27001:2022 certificate\"\n  downloadable: true\n- name: ISO/IEC 27017:2015\n  scope: cloud security\n  evidence: https://www.accredify.io/security — \"Download ISO 27017:2015 certificate\"\n  downloadable: true\n- name: ISO/IEC 27018:2019\n\
  \  scope: protection of PII in public clouds\n  evidence: https://www.accredify.io/security — \"Download ISO 27018:2019 certificate\"\n  downloadable: true\n- name: CSA STAR CAIQ\n  evidence: https://www.accredify.io/security — \"CSA STAR CAIQ website\"\n- name: ISO 22301\n  scope: business continuity management\n  evidence: https://www.accredify.io/multi-standard-flexibility\n- name: IMDA Data Protection Trustmark\n  jurisdiction: Singapore\n  evidence: https://www.accredify.io/multi-standard-flexibility\nregulatory:\n- name: Singapore Personal Data Protection Act (PDPA)\n  evidence: https://www.accredify.io/multi-standard-flexibility, https://www.accredify.io/data-protection-notice\ncontrols_published:\n  hosting: >-\n    AWS data centres in Singapore or Australia where applicable; AWS certified ISO 27001,\n    PCI DSS Service Provider Level 1 and/or SOC 2.\n  encryption_in_transit: HTTPS/TLS 1.2 or higher over public networks\n  encryption_at_rest: AES-256 in AWS\n  network: Web Application\
  \ Firewall in front of every endpoint, multi-zone architecture, IDS/IPS, DDoS mitigation\n  vulnerability_management: network vulnerability scanning plus an annual third-party penetration test of the production network\n  access_control: least privilege, need-to-know, multi-factor authentication for production network access\n  sdlc: OWASP Top 10 controls, automated unit testing, code coverage review, manual peer review, separate test/staging/production environments\n  continuity: business continuity and disaster recovery plans, cross-AZ replication, service clustering\n  vendor_management: security reviews of third-party vendors with access to systems or Service Data\n  status_page: https://status.accredify.io/\ngaps:\n- No /.well-known/security.txt on any Accredify host (all probed hosts returned 404).\n- No vulnerability disclosure policy, bug bounty programme, or named security contact address.\n- No SOC 2 report of Accredify's own; the SOC 2 reference is to AWS as the underlying hosting\
  \ provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accredify0604/refs/heads/main/security/accredify0604-trust-center.yml
summary_line: ISO/IEC 27001:2022, ISO/IEC 27017:2015, ISO/IEC 27018:2019, CSA STAR CAIQ, ISO 22301, IMDA Data Protection Trustmark
tags:
- Company
- Verifiable Credentials
- Digital Credentials
- Identity
- Document Verification
- Credentialing
- Education
- Healthcare
- Trust
- OpenBadges
- OID4VCI
- Singapore
trust_url: https://www.accredify.io/security
---
