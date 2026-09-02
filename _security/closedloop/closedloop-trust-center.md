---
api_specs:
- filename: closedloop-public-api-openapi.yaml
  format: yaml
  label: ClosedLoop AI REST API
  slug: closedloop-ai-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/openapi/closedloop-public-api-openapi.yaml
certifications:
- SOC 2 Type II
- ISO 27001
- PCI DSS
- HIPAA
- FedRAMP
description: ''
kind: trust-center
layout: security
name: Closedloop Trust Center
name_suffix: Trust Center
overview: ClosedLoop AI maintains a public trust center documenting SOC 2 Type II, ISO 27001, PCI DSS, HIPAA, and FedRAMP compliance.
provider_name: ClosedLoop AI
provider_slug: closedloop
slug: closedloop-trust-center
source_filename: closedloop-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: https://closedloop.sh/pricing, https://closedloop.sh/docs/guides/vendor-listing,\n  https://trust.closedloop.sh\nnote: >-\n  probe-security-programs.py returned trust=none because trust.closedloop.sh renders entirely\n  client-side and served no readable certification text to an anonymous fetch. It IS a real trust\n  surface -- this file records what the provider publishes in machine-readable-adjacent form\n  elsewhere on its own site, with each claim's source and status.\ntrust_center:\n  url: https://trust.closedloop.sh\n  status: 200\n  readable: false\n  readable_detail: >-\n    Returns a Next.js SPA titled \"Trust Vault\" with no server-rendered content. No certification\n    names, no document list and no report-request flow were readable without executing JavaScript.\n    Recorded honestly: the page exists and 200s, but a machine cannot read it.\n  linked_from_site: not-found\n  linked_from_site_detail: >-\n    No link\
  \ to trust.closedloop.sh was found from the marketing navigation, the docs, or the\n    vendor-listing guide. The subdomain was discovered by probe, not by following a first-party\n    link.\ncertifications:\n- name: SOC 2 Type II\n  claimed: true\n  source: https://closedloop.sh/pricing\n  source_status: 200\n  evidence: >-\n    Listed as \"Included\" on Free, Pay as you go and Enterprise in the published plan-comparison\n    table, and again in the \"On every plan\" summary block.\n  report_public: false\n  report_note: The attestation report itself is not published; no request flow was readable.\n- name: ISO 27001\n  claimed: false\n- name: PCI DSS\n  claimed: false\n  note: Not applicable -- ClosedLoop AI processes no cardholder data.\n- name: HIPAA\n  claimed: false\n- name: FedRAMP\n  claimed: false\nprivacy_program:\n  vendor_listing_page: https://closedloop.sh/docs/guides/vendor-listing\n  vendor_listing_status: 200\n  vendor_listing_note: >-\n    A genuinely unusual artifact:\
  \ a documentation page written FOR the buyer's security, privacy or\n    procurement team, giving the legal entity, registered address, processor role, contacts, data\n    categories and every policy link in a copy-paste block. Most providers make a buyer assemble\n    this from a PDF.\n  legal_entity: ClosedLoop Labs LLC, doing business as ClosedLoop AI\n  registered_address: 7901 4th St N Ste 300, St. Petersburg, FL 33702, United States\n  role: Data processor / vendor\n  privacy_contact: dpo@closedloop.sh\n  support_contact: support@closedloop.sh\n  documents:\n  - name: Privacy Policy\n    url: https://closedloop.sh/privacy\n    status: 200\n  - name: Data Processing Agreement\n    url: https://closedloop.sh/dpa\n    status: 200\n  - name: Subprocessors\n    url: https://closedloop.sh/subprocessors\n    status: 200\n  - name: AI Terms\n    url: https://closedloop.sh/ai-terms\n    status: 200\n  - name: Terms of Service\n    url: https://closedloop.sh/terms\n    status: 200\ndata_residency:\n\
  \  regions: [us, eu]\n  selection: chosen during onboarding, per workspace\n  guarantee: >-\n    \"During normal operations, EU workspace data does not leave the EU region.\" Carried through\n    every surface -- app (eu.app), REST API (eu.api), MCP (eu.mcp), SCIM and SSO all have EU\n    equivalents.\n  source: https://closedloop.sh/docs/guides/vendor-listing\naccess_posture:\n  read_only_connections: true\n  read_only_source: https://closedloop.sh/pricing\n  read_only_detail: >-\n    \"Read-only connections\" is listed as an on-every-plan property, and the /v1 API is GET-only,\n    which corroborates it from the contract side rather than from marketing alone.\nenterprise_controls:\n  sso: [Okta OIDC, Google Workspace SAML, Microsoft Entra ID SAML]\n  provisioning: SCIM 2.0 (Okta, Entra ID) with Group Push and role entitlements\n  offboarding: Global Token Revocation endpoint (Okta Universal Logout)\n  plan_gate: Enterprise\n  cross_ref: conformance/closedloop-conformance.yml\nvulnerability_disclosure:\n\
  \  published: false\n  probes:\n  - url: https://closedloop.sh/.well-known/security.txt\n    status: 404\n  - url: https://api.closedloop.sh/.well-known/security.txt\n    status: 404\n  - url: https://docs.closedloop.sh/.well-known/security.txt\n    status: 404\n  - url: https://closedloop.sh/security.txt\n    status: 404\n  - url: https://closedloop.sh/security\n    status: 404\n  detail: >-\n    No security.txt on any host, no /security page, no bug-bounty program found on HackerOne,\n    Bugcrowd or Intigriti, and no disclosure policy in the docs. A researcher who finds a\n    vulnerability has no published channel other than support@closedloop.sh. This is the clearest\n    single gap in an otherwise strong security posture, and it is cheap for the provider to close.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/closedloop/refs/heads/main/security/closedloop-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001, PCI DSS, HIPAA, FedRAMP
tags:
- Product Intelligence
- Customer Feedback
- Voice of Customer
- Product Management
- Agentic AI
- MCP
- SaaS analytics
- A2A
- SCIM
- Product Discovery
trust_url: ''
---
