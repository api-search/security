---
certifications:
- SOC 1
- SOC 2
- ISO/IEC 27001
- ISO/IEC 27017
- ISO/IEC 27018
- ISO 22301
- ISO 9001
- PCI DSS
- FedRAMP
- CSA STAR
- TISAX
- BSI C5
- IRAP
- ENS
- GDPR
description: SAP operates a company-level Trust Center with a searchable compliance document library. The automated probe in probe-security-programs.py returned no hit because www.sap.com answers 403 to its user agent; a re-fetch with full browser headers returned 200 on both the trust center and the certifications page, so this was recorded by hand from that fetch.
kind: trust-center
layout: security
name: Sap Bw Trust Center
name_suffix: Trust Center
overview: SAP BW maintains a public trust center documenting SOC 1, SOC 2, ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018, ISO 22301, ISO 9001, PCI DSS, FedRAMP, CSA STAR, TISAX, BSI C5, IRAP, ENS, and GDPR compliance.
provider_name: SAP BW
provider_slug: sap-bw
slug: sap-bw-trust-center
source_filename: sap-bw-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nprobe: true\nurl: https://www.sap.com/about/trust-center.html\nhttp_status: 200\ndescription: >-\n  SAP operates a company-level Trust Center with a searchable compliance\n  document library. The automated probe in probe-security-programs.py\n  returned no hit because www.sap.com answers 403 to its user agent; a\n  re-fetch with full browser headers returned 200 on both the trust center\n  and the certifications page, so this was recorded by hand from that fetch.\npages:\n  - name: SAP Trust Center\n    url: https://www.sap.com/about/trust-center.html\n    status: 200\n  - name: Certifications and Compliance\n    url: https://www.sap.com/about/trust-center/certification-compliance.html\n    status: 200\n  - name: Report a Security Issue (Security Incident Management)\n    url: https://www.sap.com/report-a-vulnerability\n    status: 200\n    resolves_to: https://www.sap.com/about/trust-center/security/incident-management.html\n  - name:\
  \ SAP Cloud Service Status\n    url: https://www.sap.com/about/trust-center/cloud-service-status.html\n    status: 200\ncertifications:\n  - SOC 1\n  - SOC 2\n  - ISO/IEC 27001\n  - ISO/IEC 27017\n  - ISO/IEC 27018\n  - ISO 22301\n  - ISO 9001\n  - PCI DSS\n  - FedRAMP\n  - CSA STAR\n  - TISAX\n  - BSI C5\n  - IRAP\n  - ENS\n  - GDPR\nevidence:\n  - source: https://www.sap.com/about/trust-center/certification-compliance.html\n    http_status: 200\n    bytes: 258067\n    keywords:\n      - SOC 1\n      - SOC 2\n      - ISO/IEC 27001\n      - ISO/IEC 27017\n      - ISO/IEC 27018\n      - ISO 22301\n      - PCI DSS\n      - FedRAMP\n      - CSA STAR\n      - TISAX\n      - C5\n      - IRAP\n      - ENS\n    excerpt: >-\n      \"Compliance offerings from SAP - Explore our certificates, reports, and\n      attestations.\" SAP also publishes a SOC & C5 performance calendar\n      committing SOC 1 reports within 90 days of each performance period.\nscope_caveat: >-\n  These are SAP corporate/cloud\
  \ attestations. SAP BW/4HANA deployed\n  on-premises inherits none of them - the customer runs the system and owns\n  its own certification scope. SAP BW in SAP Business Data Cloud, being an\n  SAP-operated cloud service, does fall inside SAP's cloud compliance scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-bw/refs/heads/main/security/sap-bw-trust-center.yml
summary_line: SOC 1, SOC 2, ISO/IEC 27001, ISO/IEC 27017, ISO/IEC 27018, ISO 22301, ISO 9001, PCI DSS, FedRAMP, CSA STAR, TISAX, BSI C5, IRAP, ENS, GDPR
tags:
- Business Intelligence
- Data Warehousing
- Enterprise
- ETL
- SAP
trust_url: https://www.sap.com/about/trust-center.html
---
