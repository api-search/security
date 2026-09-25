---
api_specs:
- filename: openapi-productionserver
  format: yaml
  label: MATLAB Production Server RESTful API
  slug: matlab-production-server-restful-api
  spec_type: OpenAPI
  url: https://github.com/mathworks-ref-arch/openapi-productionserver
certification_count: 3
certifications:
- SOC 3
- SOC 2 Type II
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Matlab Trust Center
name_suffix: Trust Center
overview: MATLAB maintains a public trust center documenting SOC 3, SOC 2 Type II, and ISO 27001 compliance.
provider_name: MATLAB
provider_slug: matlab
slug: matlab-trust-center
source_filename: matlab-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "specification: API Commons Trust Center\nspecificationVersion: '0.1'\nprovider: MATLAB\nproviderId: matlab\ngenerated: '2026-09-14'\nmethod: searched\nsource: https://www.mathworks.com/company/trust-center.html\nurl: https://www.mathworks.com/company/trust-center.html\nnote: >-\n  probe-security-programs.py reported trust=none because the trust centre is at\n  /company/trust-center.html rather than a /trust or /security path, and www.mathworks.com answers a\n  default crawler UA with HTTP 403. Recorded here from the page itself.\ncertifications:\n  - name: SOC 3\n    status: published\n    evidence: https://www.mathworks.com/content/dam/mathworks/policies/2024-soc-3-report.pdf\n    note: The trust centre links a dated SOC 3 report for the MathWorks Cloud-Based Applications System; SOC 3 is the publicly distributable form of the SOC 2 examination.\n  - name: SOC 2 Type II\n    status: on-request\n    evidence: https://www.mathworks.com/company/trust-center.html\n    note: Stated\
  \ as completed; the full report is released to customers through MathWorks Customer Support rather than published.\n  - name: ISO 27001\n    status: not-certified\n    evidence: https://www.mathworks.com/company/trust-center.html\n    note: >-\n      MathWorks describes its information security programme as based on industry-standard frameworks\n      including ISO 27001, but does NOT claim certification and the trust centre names no certificate.\n      Recorded as not-certified deliberately — \"based on\" is not \"certified to\".\ncompliance_programs:\n  - { name: GDPR, status: documented, artifact: GDPR subprocessor list (on request) }\n  - { name: Data Processing Agreement, status: on-request }\n  - { name: HECVAT, status: on-request, note: Higher Education Community Vendor Assessment Toolkit — the education-sector diligence questionnaire. }\n  - { name: EU Standard Contractual Clauses, status: documented }\n  - { name: UK International Data Transfer Addendum, status: documented }\n\
  not_claimed:\n  - HIPAA\n  - PCI DSS\n  - FedRAMP\n  - CSA STAR\n  - ISO 27001 (certification)\ndocuments:\n  - { name: Information Security Practices, url: \"https://www.mathworks.com/content/dam/mathworks/policies/mathworks-Information-security-practices.pdf\" }\n  - { name: Vulnerability Disclosure Policy, url: \"https://www.mathworks.com/company/aboutus/policies_statements/vulnerability-disclosure-policy.html\" }\n  - { name: Privacy Policy, url: \"https://www.mathworks.com/company/aboutus/policies_statements/privacy-policy.html\" }\n  - { name: Data Privacy FAQ, url: \"https://www.mathworks.com/company/trust-center/privacy-faq.html\" }\n  - { name: Certifications and Representations, url: \"https://www.mathworks.com/company/aboutus/policies_statements/cert_rep.html\" }\nincident_disclosure:\n  published: true\n  note: The trust centre links a public write-up of the May 2025 ransomware incident — disclosure of a real incident rather than only a policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matlab/refs/heads/main/security/matlab-trust-center.yml
summary_line: SOC 3, SOC 2 Type II, ISO 27001
tags:
- Data Analysis
- Engineering
- Machine Learning
- Numerical Analysis
- Scientific Computing
trust_url: https://www.mathworks.com/company/trust-center.html
---
