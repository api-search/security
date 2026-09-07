---
api_specs:
- filename: configure8-c8-public-api-openapi.json
  format: json
  label: Configure8 REST API
  slug: idp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-c8-public-api-openapi.json
- filename: configure8-catalog-entities-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Entities API
  slug: configure8-catalog-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-entities-api-openapi.yml
- filename: configure8-catalog-relations-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Relations API
  slug: configure8-catalog-relations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-relations-api-openapi.yml
- filename: configure8-deployments-api-openapi.yml
  format: yaml
  label: Configure8 Deployments API
  slug: configure8-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-deployments-api-openapi.yml
- filename: configure8-scorecards-api-openapi.yml
  format: yaml
  label: Configure8 Scorecards API
  slug: configure8-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-scorecards-api-openapi.yml
- filename: configure8-users-api-openapi.yml
  format: yaml
  label: Configure8 Users API
  slug: configure8-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-users-api-openapi.yml
certification_count: 1
certifications:
- SOC 2
description: configure8 does not run a hosted trust centre (no Vanta/Drata/SafeBase portal, no downloadable evidence library). What it publishes is a first-party security document inside its own product documentation, plus a named certification repeated in the site footer. The report itself is available on request, not for download.
kind: trust-center
layout: security
name: Configure8 Trust Center
name_suffix: Trust Center
overview: Configure8 maintains a public trust center documenting SOC 2 compliance.
provider_name: Configure8
provider_slug: configure8
slug: configure8-trust-center
source_filename: configure8-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://configure8.io/docs-sub/configure8-product-docs/fundamentals/security;\n  https://configure8.io/pricing;\n  https://configure8.io/privacy/policy\ndescription: >-\n  configure8 does not run a hosted trust centre (no Vanta/Drata/SafeBase portal, no\n  downloadable evidence library). What it publishes is a first-party security document\n  inside its own product documentation, plus a named certification repeated in the site\n  footer. The report itself is available on request, not for download.\ntrust_center_hosted: false\nsecurity_page: https://configure8.io/docs-sub/configure8-product-docs/fundamentals/security\ncertifications:\n- name: SOC 2\n  framework: AICPA Trust Services Criteria\n  status: claimed by the provider\n  evidence: >-\n    \"configure8 is proud to hold SOC2 certification, a testament to our unwavering\n    commitment to security.\" The same page states configure8 engages independent security\n \
  \   experts and \"collaborate[s] with an impartial auditor to maintain an up-to-date SOC 2\n    report.\" The site footer under RESOURCES > Security also reads \"SOC2 Certified\".\n  report_available: on request\n  report_public: false\n  evidence_url: https://configure8.io/docs-sub/configure8-product-docs/fundamentals/security\nprograms:\n- name: Responsible Disclosure\n  url: https://configure8.io/responsible-disclosure\n  bug_bounty: false\n  safe_harbour: >-\n    \"We do not take legal action against researchers who report vulnerabilities to us in a\n    responsible and ethical manner, following the guidelines below.\"\n  scope: >-\n    \"Our Responsible Disclosure Program encompasses app.configure8.io.\" — the single host\n    named, and the one that returned NXDOMAIN when probed on 2026-09-05.\n  submission: security contact address published on the page, with a PGP public key offered\n    for encrypting sensitive reports\n  restrictions: >-\n    No brute force, no spamming, no automated\
  \ vulnerability scanners; do not exploit a\n    finding to reach data that is not yours; keep details confidential until fixed.\n  artifact: security/configure8-vulnerability-disclosure.yml\nprivacy:\n  policy: https://configure8.io/privacy/policy\n  ccpa_do_not_sell: https://configure8.io/privacy/donotsell\n  terms: https://configure8.io/tos.pdf\n  terms_note: Terms of Service are distributed as a PDF rather than a web page.\nnot_found:\n- ISO 27001\n- PCI DSS\n- HIPAA\n- FedRAMP\n- GDPR certification or DPA published for download\n- a machine-readable security.txt on any resolvable host\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/security/configure8-trust-center.yml
summary_line: SOC 2
tags:
- Catalog
- Cloud Cost
- Developer Experience
- DevOps
- Internal Developer Portal
- Platform Engineering
- Scorecards
- Self-Service
- Service Catalog
- SRE
trust_url: ''
---
