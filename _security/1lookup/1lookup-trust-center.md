---
certifications: []
description: '1Lookup''s /security page is its trust surface: a single public page covering compliance posture, security controls, infrastructure, data lifecycle and incident response. There is no separate trust.1lookup.io portal, no downloadable report library and no third-party audit certification. The page is unusually honest about that — each compliance item is explicitly labelled self-assessed, inherited via Stripe, or internal.'
kind: trust-center
layout: security
name: 1Lookup Trust Center
name_suffix: Trust Center
overview: 1Lookup maintains a public trust center covering its security and compliance posture.
provider_name: 1Lookup
provider_slug: 1lookup
slug: 1lookup-trust-center
source_filename: 1lookup-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nprobe: true\nurl: https://www.1lookup.io/security\ndescription: >-\n  1Lookup's /security page is its trust surface: a single public page covering compliance posture,\n  security controls, infrastructure, data lifecycle and incident response. There is no separate\n  trust.1lookup.io portal, no downloadable report library and no third-party audit certification. The\n  page is unusually honest about that — each compliance item is explicitly labelled self-assessed,\n  inherited via Stripe, or internal.\nsubdomain_probed:\n  - {url: 'https://www.1lookup.io/trust', status: 404}\n  - {url: 'https://www.1lookup.io/compliance', status: 404}\n  - {url: 'https://www.1lookup.io/dpa', status: 404}\ncertifications: []\ncompliance_programs:\n  - {name: GDPR, status: self-assessed, detail: 'EU General Data Protection Regulation; data subject rights supported, Standard Contractual Clauses for transfers.'}\n  - {name: CCPA/CPRA, status: self-assessed,\
  \ detail: 'California Consumer Privacy Act as amended by CPRA; includes an opt-out of sharing for advertising.'}\n  - {name: PCI DSS, status: inherited, detail: 'Card payments handled by Stripe (PCI DSS Level 1). 1Lookup does not store full card numbers.'}\n  - {name: Internal Security Policies, status: internal, detail: 'Documented access control, encryption and incident response policies, reviewed at least annually.'}\ncontrols:\n  encryption:\n    at_rest: AES-256\n    in_transit: TLS 1.3\n    key_management: AWS KMS with automatic rotation\n    database: Transparent Data Encryption (TDE)\n  access:\n    authentication: Multi-factor authentication (MFA)\n    authorization: Role-based access control (RBAC)\n    api: Bearer token authentication\n    session: Secure JWT with refresh tokens\n  infrastructure:\n    cloud: AWS with VPC isolation and private subnets\n    network: Web Application Firewall (WAF), network ACLs, security groups\n    ddos: Cloudflare Enterprise\n    vulnerability_scanning:\
  \ Automated daily scans\n    application: OWASP Top 10 protection, input validation, API rate limiting\n  monitoring:\n    siem: 24/7 SIEM with alerts\n    audit_logging: Immutable audit trail\n    incident_response: Automated response playbooks\n    control_review: Internal review, at least annually\ndata_handling:\n  retention: Automatic deletion after 30 days\n  minimization: No personal data stored beyond validation requirements\n  sharing: No data sharing with third parties (as stated)\n  user_control: Download all your data; delete data at any time; granular privacy controls\nprivacy:\n  privacy_policy: https://www.1lookup.io/privacy\n  terms: https://www.1lookup.io/terms\ngaps:\n  - No SOC 2 Type II, ISO 27001 or other independent audit certification.\n  - No third-party trust portal or document-request workflow.\n  - No published DPA/subprocessor list at a discoverable URL.\nevidence:\n  - {source: 'https://www.1lookup.io/security', keywords: [security & compliance, gdpr, ccpa,\
  \ pci dss, soc, encryption, incident response]}\nx-evidence:\n  - url: https://www.1lookup.io/security\n    http_status: 200\n    fetched: '2026-08-09'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1lookup/refs/heads/main/security/1lookup-trust-center.yml
summary_line: trust center published
tags:
- Phone Validation
- Email Validation
- IP Intelligence
- Fraud and Risk
- Data Enrichment
- B2B contact & company data
- SEO / web analytics
- Audio Transcription
- MCP / agent-native
- REST API
trust_url: https://www.1lookup.io/security
---
