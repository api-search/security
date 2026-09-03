---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Big Picture Medical Authentication
name_suffix: Authentication
oauth_flows: []
overview: Big Picture Medical declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Big Picture Medical
provider_slug: big-picture-medical
scheme_count: 0
schemes: []
slug: big-picture-medical-authentication
source_filename: big-picture-medical-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/544327769943197\napi_authentication_documented: false\npointer_withheld: true\npointer_withheld_reason: >-\n  NO Authentication pointer is emitted into apis.yml from this file, deliberately. The\n  ergonomics check that reads type: Authentication is asking whether an integrator can\n  learn how to authenticate against the API. Nothing below answers that. Everything here\n  is workforce and tenant access control that Big Picture Medical published in a\n  procurement questionnaire — no scheme, no header name, no token endpoint, no key\n  format, no scope model, no example request. Wiring the pointer would credit the company\n  with API auth documentation it has not published.\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  note: derive-authentication.py found 0 security schemes — there is no OpenAPI in this repo\nschemes: []\npublished_access_model:\n\
  \  api_access: >-\n    \"Authenticated/Authorised users can register system/service to access the platform.\n    Authenticated/Authorised users can manage and execute workflows via platform APIs.\"\n    (G-Cloud 14, \"What users can and can't do using the API\")\n  api_documentation: 'Yes, per the same listing. Format: PDF. The PDF is not published;\n    it reaches customers through onboarding.'\n  api_sandbox: 'Yes — G-Cloud 14 answers \"API sandbox or test environment: Yes\". No public\n    sandbox URL, signup, or test credentials are published, so it is reachable only under\n    contract. Recorded here rather than in a sandbox/ artifact, because nothing about it\n    is usable by a reader.'\n  user_authentication: 2-factor authentication\n  management_access: >-\n    Role-based access control with unique credentials, multi-factor authentication,\n    environment access limited to VPNs, regular audits, encryption and secure protocols in\n    transit.\n  identity_federation: >-\n    \"\
  Identity federation with existing provider (for example Google Apps)\" is offered for\n    MANAGEMENT access. This is workforce SSO, not an API identity surface, and no OIDC\n    discovery document is served (see well-known/big-picture-medical-well-known.yml).\n  audit: >-\n    Users obtain audit information by contacting the support team; user, supplier and\n    system audit data retained at least 12 months.\ndiscovery_probes:\n- url: https://www.bigpicturemedical.com/.well-known/openid-configuration\n  status: 404\n- url: https://www.bigpicturemedical.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://www.bigpicturemedical.com/.well-known/oauth-protected-resource\n  status: 404\n- url: https://api.bigpicturemedical.com/\n  status: <no response>\n- url: https://docs.bigpicturemedical.com/\n  status: 200 at https://www.google.com/a/bigpicturemedical.com/ServiceLogin — the docs\n    hostname is a Google Workspace Drive alias and demands a bigpicturemedical.com account\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/big-picture-medical/refs/heads/main/authentication/big-picture-medical-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Healthcare
- Health Care
- Electronic Health Records
- openEHR
- FHIR
- HL7
- Interoperability
- Clinical Data
- Care Pathways
- Workflow
- Orchestration
- No Code
- NHS
- United Kingdom
---
