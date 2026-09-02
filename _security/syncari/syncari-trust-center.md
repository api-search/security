---
certifications:
- SOC 2 Type II
- HIPAA
- GDPR
- CCPA
- Standard Contractual Clauses (SCCs)
- EU-US Privacy Shield
- GLBA
description: Syncari has no dedicated trust-center subdomain (trust.syncari.com and security.syncari.com do not resolve) and no machine-readable compliance surface. It publishes two prose security pages that name real certifications and practices. Everything below is quoted or paraphrased from those two pages; nothing is inferred.
kind: trust-center
layout: security
name: Syncari Trust Center
name_suffix: Trust Center
overview: Syncari maintains a public trust center documenting SOC 2 Type II, HIPAA, GDPR, CCPA, Standard Contractual Clauses (SCCs), EU-US Privacy Shield, and GLBA compliance.
provider_name: Syncari
provider_slug: syncari
slug: syncari-trust-center
source_filename: syncari-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://syncari.com/product/security/\nname: Syncari trust and compliance posture\ndescription: >-\n  Syncari has no dedicated trust-center subdomain (trust.syncari.com and security.syncari.com do not resolve) and\n  no machine-readable compliance surface. It publishes two prose security pages that name real certifications and\n  practices. Everything below is quoted or paraphrased from those two pages; nothing is inferred.\npages:\n- url: https://syncari.com/product/security/\n  http_status: 200\n  title: Security (product page)\n- url: https://syncari.com/security-overview/\n  http_status: 200\n  title: Security Overview\ncertifications:\n- name: SOC 2 Type II\n  status: claimed\n  cadence: audited annually\n  evidence: '\"SOC 2 Type II ... audited annually\" - https://syncari.com/product/security/'\n  report_access: not published; no request form or trust portal found\n- name: HIPAA\n  status: claimed\n  form: Business Associate\
  \ Agreement available on request\n  evidence: '\"Syncari is HIPAA compliant and can provide HIPAA Business Partner Agreements\"'\n- name: GDPR\n  status: claimed\n  evidence: '\"Syncari supports Privacy Shield, SCCs, CCPA and GDPR compliance\"'\n- name: CCPA\n  status: claimed\n  evidence: same sentence as GDPR\n- name: Standard Contractual Clauses (SCCs)\n  status: claimed\n  evidence: same sentence as GDPR\n- name: EU-US Privacy Shield\n  status: claimed\n  evidence: same sentence as GDPR\n  note: >-\n    Privacy Shield was invalidated by Schrems II in 2020 and superseded by the EU-US Data Privacy Framework. Its\n    continued appearance on the page is a currency problem worth raising with the provider, not a certification.\n- name: GLBA\n  status: claimed\n  evidence: '\"complies with Gramm-Leach-Bliley Act (GLBA) of 1999 practices for securing infrastructure and applications\"'\npractices:\n- practice: Third-party penetration testing\n  detail: >-\n    \"the team performs third-party\
  \ penetration tests annually that include external break-in, and blackbox and\n    whitebox testing of our environments\"\n- practice: Vulnerability scanning\n  detail: Intensive automated and manual third-party efforts\n- practice: Encryption\n  detail: Encryption for data in transit and at rest; PII data masking and encryption\n- practice: Tenant isolation\n  detail: Logically isolates each customer's data from that of other customers\n- practice: Data use\n  detail: Customer data is not scanned for advertisements and not sold to third parties\n- practice: Access control\n  detail: Least privilege and strong authentication; Attribute Based Access Control (ABAC) is a documented product feature\nhosting:\n  primary: Google Cloud Platform\n  private_deployment:\n  - cloud: GCP\n    model: Customer's own GCP VPC, enterprise option, announced June 2026\n    docs: https://support.syncari.com/hc/en-us/sections/50402610626964-GCP-Private\n  - cloud: AWS\n    model: Public and private deployment\
  \ documentation section exists\n    docs: https://support.syncari.com/hc/en-us/sections/51821808544788-AWS-Public-and-Private\n  network:\n    ip_allowlist: https://support.syncari.com/hc/en-us/articles/360061186972-Allowlist-IP\n    tls_requirements: https://support.syncari.com/hc/en-us/articles/48005901313300-SSL-TLS-Connection-Requirements-for-Syncari-Database-Synapses\ngaps:\n- No /.well-known/security.txt on any Syncari host (all probed 404 or 401).\n- No vulnerability disclosure policy, security contact address, or bug bounty programme found; hackerone.com/syncari\n  and bugcrowd.com/syncari both return 404.\n- No trust portal, sub-processor list, or self-serve report request.\n- Certifications are prose claims on a marketing page; there is no machine-readable attestation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syncari/refs/heads/main/security/syncari-trust-center.yml
summary_line: SOC 2 Type II, HIPAA, GDPR, CCPA, Standard Contractual Clauses (SCCs), EU-US Privacy Shield, GLBA
tags:
- Company
- Master Data Management
- data-unification
- Data Integration
- iPaaS
- Data Quality
- Data Governance
- embedded-integration
- MCP
- agent-native
- Revenue Operations
- Data Synchronization
trust_url: ''
---
