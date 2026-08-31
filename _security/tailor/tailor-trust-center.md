---
certifications:
- SOC 2
- ISO 27001
- PCI DSS
- HIPAA
- FedRAMP
description: Tailor does not operate a dedicated trust-center subdomain — trust.tailor.tech and security.tailor.tech resolve only through a wildcard record and return a Fastly default body, not a trust page. The company's compliance posture is published inside the developer documentation instead, on docs.tailor.tech/reference/security, which names SOC 2 as its compliance framework.
kind: trust-center
layout: security
name: Tailor Trust Center
name_suffix: Trust Center
overview: Tailor maintains a public trust center documenting SOC 2, ISO 27001, PCI DSS, HIPAA, and FedRAMP compliance.
provider_name: Tailor
provider_slug: tailor
slug: tailor-trust-center
source_filename: tailor-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://docs.tailor.tech/reference/security\nname: Tailor trust and compliance posture\ndescription: >-\n  Tailor does not operate a dedicated trust-center subdomain — trust.tailor.tech and\n  security.tailor.tech resolve only through a wildcard record and return a Fastly default\n  body, not a trust page. The company's compliance posture is published inside the\n  developer documentation instead, on docs.tailor.tech/reference/security, which names\n  SOC 2 as its compliance framework.\ntrust_page:\n  url: https://docs.tailor.tech/reference/security\n  status: 200\n  dedicated_subdomain: false\n  subdomain_probes:\n  - url: https://trust.tailor.tech/\n    status: 200\n    note: Wildcard *.tailor.tech record answering with a Fastly default body (\"index.html\"), not a trust center.\n  - url: https://security.tailor.tech/\n    status: 200\n    note: Wildcard *.tailor.tech record answering with a Fastly default body (\"index.html\"\
  ), not a security page.\ncertifications:\n- name: SOC 2\n  authority: AICPA\n  status: claimed\n  evidence: >-\n    \"Tailor complies with SOC2, which is a compliance framework by the American Institute\n    of Certified Public Accountants' (AICPA). Potential customers can reach out to us for\n    more information.\" — https://docs.tailor.tech/reference/security\n  report_access: on request (sales gate — no self-serve report portal or NDA workflow published)\n  corroboration: >-\n    Vanta publishes a customer story describing Tailor achieving SOC 2 in 2.5 months —\n    https://www.vanta.com/customers/tailor (third-party, not used as the primary claim).\n- name: ISO 27001\n  status: not-claimed\n- name: PCI DSS\n  status: not-claimed\n- name: HIPAA\n  status: not-claimed\n- name: FedRAMP\n  status: not-claimed\nsecurity_controls:\n  encryption_at_rest: AES-256\n  encryption_in_transit: TLS\n  access_control: RBAC with automatic deprovisioning on termination\n  network: segmentation, firewalls,\
  \ intrusion detection\n  endpoint: MDM-enforced disk encryption, screen lock, patching; 24/7/365 alert monitoring\n  third_party_assessments: yes\n  ip_allowlisting: CIDR allowlists at organization, folder or application level\n  data_residency: regional cloud deployment (asia-northeast, us-west)\ndata_retention:\n  source: https://docs.tailor.tech/administration/data-retention\n  periods:\n  - data_type: Jobs and attempts (Executor)\n    retention: 30 days\n  - data_type: Executions (Function service)\n    retention: 30 days\n  - data_type: Resolver execution results\n    retention: 30 days\n  - data_type: Dataplane events\n    retention: 3 days\n  - data_type: Controlplane activity logs\n    retention: 90 days\n  note: After the retention period the data is permanently deleted and cannot be recovered.\nx-evidence:\n  fetched: '2026-08-29'\n  probes:\n  - url: https://docs.tailor.tech/reference/security.md\n    status: 200\n  - url: https://docs.tailor.tech/administration/data-retention.md\n\
  \    status: 200\n  - url: https://trust.tailor.tech/\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailor/refs/heads/main/security/tailor-trust-center.yml
summary_line: SOC 2, ISO 27001, PCI DSS, HIPAA, FedRAMP
tags:
- Company
- ERP
- Headless ERP
- Retail
- E-Commerce
- Supply Chain
- Inventory Management
- GraphQL
- gRPC
- Low-Code
- Composable Commerce
- Manufacturing
trust_url: ''
---
