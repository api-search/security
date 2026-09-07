---
certification_count: 6
certifications:
- NIST SP 800-171
- CMMC
- SOC 2 Type 2
- SOC 2 Type 3
- CIS Top 20
- FIPS 140-2
description: ''
kind: trust-center
layout: security
name: Virtualitics Trust Center
name_suffix: Trust Center
overview: Virtualitics maintains a public trust center documenting NIST SP 800-171, CMMC, SOC 2 Type 2, SOC 2 Type 3, CIS Top 20, and FIPS 140-2 compliance.
provider_name: Virtualitics
provider_slug: virtualitics
slug: virtualitics-trust-center
source_filename: virtualitics-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://virtualitics.com/security/\nchecked: '2026-09-04'\nfound: true\ntrust_center:\n  kind: published security page (not a hosted trust portal)\n  url: https://virtualitics.com/security/\n  dedicated_subdomain: false\n  probed:\n  - host: trust.virtualitics.com\n    result: NXDOMAIN\n  note: >-\n    Virtualitics does not run a Vanta/Drata/SafeBase-style trust portal. It publishes a single\n    first-party security page that names its frameworks and offers a downloadable report, which is\n    the substance a buyer needs even without the portal.\ncertifications:\n- name: NIST SP 800-171\n  status: compliant\n- name: CMMC\n  status: ready\n- name: SOC 2 Type 2\n  status: achieved\n  report_available: true\n- name: SOC 2 Type 3\n  status: in process\n  note: >-\n    As written on the page. SOC 3 is the public-report form of SOC 2; the page separately offers a\n    \"Service Organization Control 3 (SOC 3) report\" download.\n\
  - name: CIS Top 20\n  status: listed\n- name: FIPS 140-2\n  status: claimed (cryptography)\nreports_available:\n- name: SOC 3 report\n  access: download from https://virtualitics.com/security/\n- name: SOC 2 Type 2 report\n  access: referenced on the security page\ncontrol_areas:\n  product_security:\n  - Continuous internal and external vulnerability scanning\n  - Data encryption at rest and in transit\n  - Data validation\n  - Data retention\n  - Data isolation\n  - FIPS 140-2 cryptographic compliance\n  security_monitoring:\n  - Continuous network vulnerability scanning\n  - Continuous endpoint security monitoring\n  - Continuous cloud security monitoring\n  business_resiliency:\n  - Business continuity program\n  - Disaster recovery testing\n  workforce_security:\n  - Background checks\n  - Security awareness training\n  - Continuous phishing email campaigns\ngovernment_posture:\n  statement: >-\n    \"strict adherence to US Department of War security requirements and commercial security\n\
  \    standards and frameworks\", validated by \"external and independent assessments of our\n    cybersecurity risk management program\".\n  networks: [NIPR, SIPR, JWICS]\n  platforms: [ADVANA, ODIN]\n  source: https://virtualitics.com/company-overview/\ngaps:\n- No FedRAMP or StateRAMP authorization is named.\n- No ISO/IEC 27001 certification is named.\n- No CMVP certificate number is given for the FIPS 140-2 claim.\n- No sub-processor list, data-residency statement or pen-test cadence is published.\n- No security.txt — see security/virtualitics-vulnerability-disclosure.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtualitics/refs/heads/main/security/virtualitics-trust-center.yml
summary_line: NIST SP 800-171, CMMC, SOC 2 Type 2, SOC 2 Type 3, CIS Top 20, FIPS 140-2
tags:
- Company
- Artificial Intelligence
- Data Analytics
- Data Visualization
- Machine Learning
- Defense
- Government
- Python
- SDK
- Command Line Interface
trust_url: ''
---
