---
api_specs:
- filename: sonarqube-issues-api-openapi.yml
  format: yaml
  label: SonarQube Issues API
  slug: sonarqube-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-issues-api-openapi.yml
- filename: sonarqube-measures-api-openapi.yml
  format: yaml
  label: SonarQube Measures API
  slug: sonarqube-measures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-measures-api-openapi.yml
- filename: sonarqube-projects-api-openapi.yml
  format: yaml
  label: SonarQube Projects API
  slug: sonarqube-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-projects-api-openapi.yml
- filename: sonarqube-quality-gates-api-openapi.yml
  format: yaml
  label: SonarQube Quality Gates API
  slug: sonarqube-quality-gates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-quality-gates-api-openapi.yml
- filename: sonarqube-rules-api-openapi.yml
  format: yaml
  label: SonarQube Rules API
  slug: sonarqube-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-rules-api-openapi.yml
- filename: sonarqube-system-api-openapi.yml
  format: yaml
  label: SonarQube System API
  slug: sonarqube-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-system-api-openapi.yml
- filename: sonarqube-users-api-openapi.yml
  format: yaml
  label: SonarQube Users API
  slug: sonarqube-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sonarqube/openapi/sonarqube-users-api-openapi.yml
certification_count: 5
certifications:
- SOC 2 Type II
- ISO/IEC 27001:2022
- ISO/IEC 27018:2019
- CSA STAR Level 1
- PCI DSS SAQ-A
description: SonarSource publishes a Vanta-hosted trust center (trust.sonarsource.com, "Sonar and Gitar Security and Data Protection", rendered 2026-11-05) listing certifications, self-assessments, penetration-test summaries and policies, with a request-access gate for the documents themselves, plus a marketing trust-center page on sonarsource.com that links it, the status page and the accessibility statement. The dossier's security-programs probe wrote nothing because the certifications are rendered client-side; they were read from the rendered page.
kind: trust-center
layout: security
name: SonarQube Trust Center
name_suffix: Trust Center
overview: SonarQube maintains a public trust center documenting SOC 2 Type II, ISO/IEC 27001:2022, ISO/IEC 27018:2019, CSA STAR Level 1, and PCI DSS SAQ-A compliance.
provider_name: SonarQube
provider_slug: sonarqube
slug: sonarqube-trust-center
source_filename: sonarqube-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://trust.sonarsource.com/\n- https://www.sonarsource.com/trust-center/\n- https://www.sonarsource.com/legal/security-tom/\nurl: https://trust.sonarsource.com/\nplatform: vanta\nname: Sonar Security Trust Center\ndescription: SonarSource publishes a Vanta-hosted trust center (trust.sonarsource.com, \"Sonar and Gitar Security\n  and Data Protection\", rendered 2026-11-05) listing certifications, self-assessments, penetration-test summaries\n  and policies, with a request-access gate for the documents themselves, plus a marketing trust-center page on sonarsource.com\n  that links it, the status page and the accessibility statement. The dossier's security-programs probe wrote nothing\n  because the certifications are rendered client-side; they were read from the rendered page.\ncontact: security@sonarsource.com\ncertifications:\n- SOC 2 Type II\n- ISO/IEC 27001:2022\n- ISO/IEC 27018:2019\n- CSA STAR Level 1\n- PCI DSS SAQ-A\n\
  penetration_tests:\n- SonarQube Server October 2026 Pentest Executive Summary.pdf\n- SonarQube Cloud May 2026 Pentest Executive Summary.pdf\n- SonarQube Hunter Agent August 2026 Pentest Executive Summary.pdf\n- SonarQube Remediation Agent PenTest June 2026.pdf\nrelated:\n  status_page: https://status.sonarqube.com/\n  accessibility_statement: https://www.sonarsource.com/accessibility/\n  subprocessors: https://www.sonarsource.com/legal/sub-processors/\n  security_measures: https://www.sonarsource.com/legal/security-tom/\n  vulnerability_reporting: '\"please follow our Responsible Vulnerability Disclosure process to report it to our\n    security team\" (https://www.sonarsource.com/trust-center/); contact security@sonarsource.com. No standalone\n    disclosure-policy page or security.txt was found on sonarsource.com during this pass.'\nplatform_evidence: trust.sonarsource.com serves the Vanta Trust Center app (data-signature-manifest-url assets.vanta.com\n  in the page HTML, 2026-11-05)\n\
  frameworks:\n- name: SOC 2 Type II\n  evidence: '\"Sonar SOC 2 Type II Report Nov 2025 - Oct 2026.pdf\" listed under Certifications and Attestations on\n    https://trust.sonarsource.com/; \"Sonar maintains both ISO 27001:2022 certification and SOC 2 Type II attestation\n    for all products and services\" (https://www.sonarsource.com/trust-center/)'\n  scope: all products and services\n- name: ISO/IEC 27001:2022\n  evidence: '\"ISO 27001:2022 Certificate\" and \"ISO 27001 SoA\" listed on https://trust.sonarsource.com/'\n  scope: all products and services\n- name: ISO/IEC 27018:2019\n  evidence: '\"Sonar ISO 27018 Certification\" on https://trust.sonarsource.com/; https://www.sonarsource.com/legal/security-tom/\n    \"Maintains ISO 27001:2022 certification, ISO 27018:2019 certification, and/or AICPA SOC 2 attestation.\"'\n  scope: null\n- name: CSA STAR Level 1\n  evidence: '\"CSA STAR Level 1 Registry - SonarQube Cloud\" and \"SonarQube Cloud 2026 CSA CAIQ v4.1.0\" under Self\n    Assessments\
  \ on https://trust.sonarsource.com/'\n  scope: SonarQube Cloud\n- name: PCI DSS SAQ-A\n  evidence: '\"Sonar PCI-DSS SAQ-A\" under Self Assessments on https://trust.sonarsource.com/'\n  scope: SonarQube Cloud\n"
source_yaml_url: https://artifacts.apis.io/sonarqube/security/sonarqube-trust-center.yml
summary_line: SOC 2 Type II, ISO/IEC 27001:2022, ISO/IEC 27018:2019, CSA STAR Level 1, PCI DSS SAQ-A
tags:
- Code Quality
- Developer Tools
- DevOps
- Security
- Static Analysis
- Code Security
- SAST
trust_url: https://trust.sonarsource.com/
---
