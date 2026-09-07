---
certification_count: 2
certifications:
- audited_certifications
- note
description: ''
kind: trust-center
layout: security
name: Acquco Trust Center
name_suffix: Trust Center
overview: Acquco maintains a public trust center documenting audited_certifications and note compliance.
provider_name: Acquco
provider_slug: acquco
slug: acquco-trust-center
source_filename: acquco-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://sellerfusion.io/security\nname: Acquco / Sellerfusion Security & Trust\ncompany: Acquco\ntrust_center:\n  published: true\n  url: https://sellerfusion.io/security\n  hosted_on: first-party page (not a third-party trust platform)\n  dedicated_subdomain: false\n  probed:\n  - url: https://trust.acqu.co/\n    status: 0\n    note: host does not resolve\n  - url: https://status.sellerfusion.io/\n    status: 404\n    note: >-\n      resolves to a Kubernetes ingress serving a self-signed \"Kubernetes Ingress Controller\n      Fake Certificate\" and a 404 — not a status page\n  page_last_updated: '2026-04-08'\ncertifications:\n  audited_certifications: []\n  note: >-\n    No SOC 2, ISO 27001, PCI DSS, HIPAA or FedRAMP certification is claimed anywhere on the\n    page. What is published is a self-attested program aligned to frameworks, plus\n    marketplace and privacy-regulation compliance.\nframeworks_referenced:\n- id: nist-sp-800-53\n\
  \  name: NIST SP 800-53\n  claim: security program and incident response plan built on / structured against it\n  audited: false\n- id: amazon-sp-api-security-controls\n  name: Amazon SP-API security control guidance\n  claim: security program built on it\n  audited: false\ncompliance_programs:\n- id: amazon-dpp\n  name: Amazon Data Protection Policy\n  status: claimed compliant\n  detail: >-\n    Registered developer in the Amazon Selling Partner Appstore; compliant with the Amazon\n    Data Protection Policy, SP-API security control guidance and the Solution Provider\n    Agreement.\n- id: gdpr\n  name: General Data Protection Regulation\n  status: claimed compliant\n  detail: 72-hour supervisory-authority notification commitment for EU personal data breaches.\n- id: ccpa\n  name: California Consumer Privacy Act\n  status: claimed compliant\n  detail: California residents exercise privacy rights via privacy@sellerfusion.io.\nsecurity_program:\n  encryption_at_rest: AES-256\n  encryption_in_transit:\
  \ TLS 1.2 or higher\n  key_management: dedicated key management systems, periodic rotation\n  access_control: least privilege, MFA on all accounts, periodic access reviews\n  vulnerability_management: ongoing scanning, periodic third-party penetration testing\n  network: segmented networks, IDS/IPS, anti-malware, credential-exposure monitoring\n  logging: centralized log collection, retention per compliance requirements\n  personnel: security awareness training, background checks, confidentiality agreements\ndata_retention:\n  policy_published: true\n  pii: retained only as long as necessary per the Amazon Data Protection Policy, then securely deleted\n  deletion_sla: permanent secure deletion within 30 days of a deletion request unless legally mandated\n  backups: AES-256 encrypted at rest, geographically replicated, same retention as primary data\n  classification: PII tagged separately from non-PII at the storage layer\ncontacts:\n  security: security@sellerfusion.io\n  privacy: privacy@sellerfusion.io\n\
  x-evidence:\n  fetched: '2026-09-06'\n  url: https://sellerfusion.io/security\n  http_status: 200\n  content_type: text/html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acquco/refs/heads/main/security/acquco-trust-center.yml
summary_line: audited_certifications, note
tags:
- Company
- E-Commerce
- Amazon
- Marketplaces
- Amazon FBA
- Aggregator
- Mergers And Acquisitions
- Seller Tools
- Analytics
- Retail
- SaaS
- New York
trust_url: ''
---
