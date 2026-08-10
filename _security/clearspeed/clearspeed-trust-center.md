---
api_specs:
- filename: clearspeed-default-api-openapi.yml
  format: yaml
  label: Clearspeed Default API
  slug: clearspeed-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearspeed/refs/heads/main/openapi/clearspeed-default-api-openapi.yml
certifications:
- SOC 2 Type 2
- ISO 27001:2022
- UK Cyber Essentials
description: ''
kind: trust-center
layout: security
name: Clearspeed Trust Center
name_suffix: Trust Center
overview: Clearspeed maintains a public trust center documenting SOC 2 Type 2, ISO 27001:2022, and UK Cyber Essentials compliance.
provider_name: Clearspeed
provider_slug: clearspeed
slug: clearspeed-trust-center
source_filename: clearspeed-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nprobe: true\nurl: https://compliance.clearspeed.com/\nplatform: SafeBase\nplatform_note: >-\n  The trust center is a SafeBase-hosted portal. Its compliance automation is stated to be\n  Drata. https://trust.clearspeed.com/ is advertised on the marketing security page but\n  did not complete a TLS handshake on 2026-08-04; https://compliance.clearspeed.com/ is\n  the host that actually serves the trust center (HTTP 200).\nlinked_from: https://www.clearspeed.com/security-commitment\ncertifications:\n- name: SOC 2 Type 2\n  document: Clearspeed - 2025 SOC 2 Type 2-Schellman.pdf\n  auditor: Schellman\n  year: 2025\n  access: gated (NDA/request flow on the trust center)\n- name: ISO 27001:2022\n  document: ISO 27001_2022_Certificate.pdf\n  access: gated\n- name: UK Cyber Essentials\n  document: UK Cyber Essentials Certificate.pdf\n  access: gated\nframeworks_claimed:\n- ISO 27001\n- ISO 27701:2019\n- SOC 2\n- GDPR\n- CCPA\n- HIPAA\n- NIST\
  \ 800-53\n- NIST 800-171\nframeworks_note: >-\n  ISO 27701:2019, HIPAA, GDPR, CCPA, NIST 800-53 and NIST 800-171 are named in trust\n  center control narratives and on the marketing security page as frameworks Clearspeed\n  aligns to or maps controls against. Only SOC 2 Type 2, ISO 27001:2022 and UK Cyber\n  Essentials are backed by a downloadable certificate/report on the portal.\ncontrol_domains_published:\n- Access Control\n- AI Governance\n- AI Security\n- App Security\n- Application Penetration Testing\n- Asset Management\n- Audit Logging\n- Backup\n- BC/DR\n- Business Continuity Plan\n- Change Management\n- Code Analysis\n- Configuration Management\n- Container Orchestration\n- Continuous Monitoring\n- Credential Management\n- Data Retention and Destruction\n- Penetration Testing\n- Responsible Disclosure\n- Software Bill of Materials (SBOM)\n- Software Development Lifecycle\n- Subprocessors\n- Vulnerability & Patch Management\ninfrastructure_disclosed:\n- Amazon Web Services\n-\
  \ Google Cloud\n- HashiCorp Vault (secrets management, KMS auto-unseal, Kubernetes \"Services\" clusters)\nsubprocessors:\n  published: partial\n  note: >-\n    A Subprocessors section exists on the trust center but the list is behind the\n    document-request flow — \"Please contact us for more details.\"\ndocument_access:\n  public_documents: false\n  flow: request/NDA through the SafeBase portal\nsecurity_contact: null\nsecurity_contact_note: >-\n  No security@ address is published on the trust center, on the marketing security page,\n  or in a security.txt (none exists on any Clearspeed host — see\n  well-known/clearspeed-well-known.yml). Reports go through the trust center contact flow.\nevidence:\n- {source: 'https://compliance.clearspeed.com/', http_status: 200, keywords: [SOC 2 Type\n      2, ISO 27001:2022, ISO 27701:2019, HIPAA, GDPR, CCPA, Drata, SafeBase, Trust Center,\n      Responsible Disclosure]}\n- {source: 'https://www.clearspeed.com/security-commitment', http_status:\
  \ 200, keywords: [\n      SOC 2, ISO 27001, GDPR, NIST 800-171, View Clearspeed Trust Center]}\n- {source: 'https://trust.clearspeed.com/', http_status: null, result: TLS handshake failure}\nx-evidence:\n  fetched: '2026-08-04'\ncross_links:\n  vulnerability_disclosure: security/clearspeed-vulnerability-disclosure.yml\n  conformance: conformance/clearspeed-conformance.yml\n  domain_security: security/clearspeed-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearspeed/refs/heads/main/security/clearspeed-trust-center.yml
summary_line: SOC 2 Type 2, ISO 27001:2022, UK Cyber Essentials
tags:
- Company
- Risk Assessment
- Fraud Detection
- Voice Analytics
- Artificial Intelligence
- Insurance
- Identity Verification
- Screening
- Security
trust_url: https://compliance.clearspeed.com/
---
