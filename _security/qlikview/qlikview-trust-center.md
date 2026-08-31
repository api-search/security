---
certifications:
- ISO/IEC 27001:2022
- ISO/IEC 27017:2015
- ISO/IEC 27018:2019
- ISO/IEC 42001:2023
- SOC 1
- SOC 2 + HITRUST CSF
- SOC 3
- HIPAA
- TISAX
- IRAP
- Cyber Essentials
- Cyber Essentials Plus
- UK G-Cloud v14
- CASA Tier 3
- C5 (German BSI)
description: Qlik's public trust and security page, the vendor trust center covering QlikView. Upgraded 2026-08-29 from the 2026-07-11 pass, which pointed only at https://security.qlik.com/ and carried a six-item certification list. security.qlik.com is the Qlik Security Trust Center where "Qlik security artifacts are available to customers" - it returned HTTP 403 to an anonymous browser-UA request on 2026-08-29, i.e. it is customer-gated. The public, anonymously readable trust page is https://www.qlik.com/us/trust (HTTP 200) and it names a much longer certification list, recorded below.
kind: trust-center
layout: security
name: Qlikview Trust Center
name_suffix: Trust Center
overview: QlikView maintains a public trust center documenting ISO/IEC 27001:2022, ISO/IEC 27017:2015, ISO/IEC 27018:2019, ISO/IEC 42001:2023, SOC 1, SOC 2 + HITRUST CSF, SOC 3, HIPAA, TISAX, IRAP, Cyber Essentials, Cyber Essentials Plus, UK G-Cloud v14, CASA Tier 3, and C5 (German BSI) compliance.
provider_name: QlikView
provider_slug: qlikview
slug: qlikview-trust-center
source_filename: qlikview-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nprobe: true\nsource: https://www.qlik.com/us/trust\nurl: https://www.qlik.com/us/trust\nprovider: QlikView\nproviderId: qlikview\ndescription: >-\n  Qlik's public trust and security page, the vendor trust center covering QlikView. Upgraded\n  2026-08-29 from the 2026-07-11 pass, which pointed only at https://security.qlik.com/ and\n  carried a six-item certification list. security.qlik.com is the Qlik Security Trust Center\n  where \"Qlik security artifacts are available to customers\" - it returned HTTP 403 to an\n  anonymous browser-UA request on 2026-08-29, i.e. it is customer-gated. The public,\n  anonymously readable trust page is https://www.qlik.com/us/trust (HTTP 200) and it names a\n  much longer certification list, recorded below.\nscope_note: >-\n  These are Qlik company and Qlik Cloud certifications. QlikView is customer-installed\n  software running on the customer's own Windows servers, so certifications that certify\
  \ a\n  HOSTED environment (FedRAMP, GovRAMP, TX-RAMP, DISA IL2/IL4, CJIS) attach to Qlik Cloud\n  Government, not to a QlikView deployment. The boundary is stated rather than blurred.\ncertifications:\n  - ISO/IEC 27001:2022\n  - ISO/IEC 27017:2015\n  - ISO/IEC 27018:2019\n  - ISO/IEC 42001:2023\n  - SOC 1\n  - SOC 2 + HITRUST CSF\n  - SOC 3\n  - HIPAA\n  - TISAX\n  - IRAP\n  - Cyber Essentials\n  - Cyber Essentials Plus\n  - UK G-Cloud v14\n  - CASA Tier 3\n  - C5 (German BSI)\ngovernment_only_certifications:\n  note: Qlik Cloud Government scope. Not applicable to an on-premises QlikView install.\n  items:\n    - FedRAMP\n    - GovRAMP\n    - TX-RAMP Level 2\n    - ITAR\n    - DISA Impact Level 2\n    - DISA Impact Level 4\n    - CJIS\ncontacts:\n  security_email: security@qlik.com\n  vulnerability_disclosure: https://hackerone.com/qlik\ngated_portal:\n  url: https://security.qlik.com/\n  status: 403\n  note: >-\n    Qlik Security Trust Center. Security artifacts (SOC reports, pen-test\
  \ summaries,\n    questionnaires) are made available to customers here; anonymous access is refused, so\n    the artifact inventory behind it could not be enumerated.\nevidence:\n  - source: https://www.qlik.com/us/trust\n    status: 200\n    fetched: '2026-08-29'\n    keywords:\n      - iso 27001\n      - iso 42001\n      - soc 2\n      - hitrust\n      - hipaa\n      - fedramp\n      - tisax\n      - c5\n  - source: https://security.qlik.com/\n    status: 403\n    fetched: '2026-08-29'\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qlikview/refs/heads/main/security/qlikview-trust-center.yml
summary_line: ISO/IEC 27001:2022, ISO/IEC 27017:2015, ISO/IEC 27018:2019, ISO/IEC 42001:2023, SOC 1, SOC 2 + HITRUST CSF, SOC 3, HIPAA, TISAX, IRAP, Cyber Essentials, Cyber Essentials Plus, UK G-Cloud v14, CASA Tier 3, C5 (German BSI)
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Discovery
- Data Visualization
- Embedded Analytics
- On Premises
- SOAP
- Guided Analytics
- Reporting
trust_url: https://www.qlik.com/us/trust
---
