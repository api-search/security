---
api_specs:
- filename: nord-security-nordstellar-enterprise-data-api-openapi.json
  format: json
  label: NordStellar Enterprise Data API
  slug: nordstellar-enterprise-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-enterprise-data-api-openapi.json
- filename: nord-security-nordstellar-company-risk-scoring-api-openapi.json
  format: json
  label: NordStellar Company Risk Scoring API
  slug: nordstellar-company-risk-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-company-risk-scoring-api-openapi.json
- filename: nord-security-nordstellar-cybersec-api-openapi.json
  format: json
  label: NordStellar Cybersec API
  slug: nordstellar-cybersec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-cybersec-api-openapi.json
- filename: nord-security-nordstellar-partners-api-openapi.json
  format: json
  label: NordStellar Partners API
  slug: nordstellar-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-partners-api-openapi.json
- filename: nord-security-nordstellar-platform-integration-api-v3-openapi.json
  format: json
  label: NordStellar Platform Integrations API
  slug: nordstellar-platform-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/openapi/nord-security-nordstellar-platform-integration-api-v3-openapi.json
certifications:
- ISO 27001
- SOC 2 Type II
- HIPAA
- PCI DSS
description: ''
kind: trust-center
layout: security
name: Nord Security Trust Center
name_suffix: Trust Center
overview: Nord Security maintains a public trust center documenting ISO 27001, SOC 2 Type II, HIPAA, and PCI DSS compliance.
provider_name: Nord Security
provider_slug: nord-security
slug: nord-security-trust-center
source_filename: nord-security-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nprobe: true\nurl: https://trust.nordlayer.com/\ntrust_centers:\n- url: https://trust.nordlayer.com/\n  product: NordLayer\n  http_status: 200\n  title: Trust Center\n  rendering: client-side (document body is JS-rendered; certification list not retrievable anonymously)\n- url: https://trust.nordpass.com/\n  product: NordPass\n  http_status: 200\n  title: Trust Center\n  rendering: client-side (document body is JS-rendered; certification list not retrievable anonymously)\n- url: https://trust.nordsecurity.com/\n  product: Nord Security (corporate)\n  http_status: 0\n  note: Host does not resolve — there is no corporate-level trust center.\ncompliance_page:\n  url: https://nordlayer.com/compliance/\n  http_status: 200\ncertifications:\n- name: ISO 27001\n  claimed_by: NordLayer\n  claim: ISO 27001 compliant\n  source: https://nordlayer.com/compliance/\n- name: SOC 2 Type II\n  claimed_by: NordLayer\n  claim: SOC 2 compliant / SOC 2 Type\
  \ II\n  source: https://nordlayer.com/compliance/\n- name: HIPAA\n  claimed_by: NordLayer\n  claim: HIPAA compliant\n  source: https://nordlayer.com/compliance/\n- name: PCI DSS\n  claimed_by: NordLayer\n  claim: PCI-DSS compliant\n  source: https://nordlayer.com/compliance/\nframeworks_supported:\n  note: >-\n    Frameworks NordLayer positions itself as helping customers meet, rather than holding certification\n    against.\n  items: [SOC 2, ISO 27001, HIPAA, NIS2, PCI DSS, GDPR]\nevidence:\n- source: https://nordlayer.com/compliance/\n  keywords: [iso 27001, soc 2, soc 2 type ii, hipaa, pci-dss, nis2, gdpr]\n  fetched: '2026-08-01'\n- source: https://trust.nordlayer.com/\n  keywords: [trust center]\n  http_status: 200\n  fetched: '2026-08-01'\n- source: https://trust.nordpass.com/\n  keywords: [trust center]\n  http_status: 200\n  fetched: '2026-08-01'\n- source: https://nordsecurity.com/\n  keywords: [iso 27001, soc 2, hipaa, gdpr]\n  fetched: '2026-08-01'\ngaps:\n- Both trust centers\
  \ render entirely client-side, so no machine-readable certification manifest exists.\n- >-\n    The published certification claims are scoped to NordLayer. NordStellar — the product that carries\n    the entire public API surface — publishes no trust center and no certification page of its own.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nord-security/refs/heads/main/security/nord-security-trust-center.yml
summary_line: ISO 27001, SOC 2 Type II, HIPAA, PCI DSS
tags:
- Cybersecurity
- Threat Intelligence
- Dark Web Monitoring
- Attack Surface Management
- Breach Intelligence
- VPN
- Password Management
- Network Security
- Zero Trust
- Privacy
- MCP
- Agent Skills
- gRPC
- Company
trust_url: https://trust.nordlayer.com/
---
