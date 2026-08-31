---
api_key_in: []
api_specs:
- filename: carnegie-mellon-university-articles-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Articles API
  slug: carnegie-mellon-university-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-articles-api-openapi.yml
- filename: carnegie-mellon-university-covidcast-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Covidcast API
  slug: carnegie-mellon-university-covidcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-covidcast-api-openapi.yml
- filename: carnegie-mellon-university-feeds-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Feeds API
  slug: carnegie-mellon-university-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-feeds-api-openapi.yml
- filename: carnegie-mellon-university-fluview-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Fluview API
  slug: carnegie-mellon-university-fluview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-fluview-api-openapi.yml
- filename: carnegie-mellon-university-forecasts-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Forecasts API
  slug: carnegie-mellon-university-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-forecasts-api-openapi.yml
- filename: carnegie-mellon-university-issues-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Issues API
  slug: carnegie-mellon-university-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-issues-api-openapi.yml
- filename: carnegie-mellon-university-journals-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Journals API
  slug: carnegie-mellon-university-journals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-journals-api-openapi.yml
- filename: carnegie-mellon-university-meta-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Meta API
  slug: carnegie-mellon-university-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-meta-api-openapi.yml
- filename: carnegie-mellon-university-notes-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Notes API
  slug: carnegie-mellon-university-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-notes-api-openapi.yml
- filename: carnegie-mellon-university-oai-pmh-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Oai Pmh API
  slug: carnegie-mellon-university-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-oai-pmh-api-openapi.yml
- filename: carnegie-mellon-university-preprints-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Preprints API
  slug: carnegie-mellon-university-preprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-preprints-api-openapi.yml
- filename: carnegie-mellon-university-vendors-api-openapi.yml
  format: yaml
  label: Carnegie Mellon University Vendors API
  slug: carnegie-mellon-university-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/openapi/carnegie-mellon-university-vendors-api-openapi.yml
auth_types:
- none
- saml
description: ''
kind: authentication
layout: security
method: probed
name: Carnegie Mellon University Authentication
name_suffix: Authentication
oauth_flows: []
overview: Carnegie Mellon University secures its APIs with none and saml across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Carnegie Mellon University
provider_slug: carnegie-mellon-university
scheme_count: 3
schemes:
- applies_to: https://api.delphi.cmu.edu/epidata
  description: The Delphi Epidata API is public, read-only and anonymous. No key, token, header or registration is required; the documentation asks only that heavy users be considerate. Probed 2026-08-19 with no credential on five endpoints, all 200.
  evidence:
    content_type: application/json
    status: 200
    url: https://api.delphi.cmu.edu/epidata/version
  name: DelphiEpidataPublic
  operator: institution
  type: none
- applies_to: https://kb.cert.org/vuls/api
  description: 'The CERT/CC Vulnerability Notes read API requires no credential. Note the failure mode: an unknown identifier returns HTTP 200 with {"error":"Content requested either does not exist or you do not have permissions to view it!"}, which conflates "not found" with "not authorized" — a client cannot distinguish a bad VU number from a permission boundary.'
  evidence:
    content_type: application/json
    status: 200
    url: https://kb.cert.org/vuls/api/421644/
  name: CERTVulnerabilityNotesPublic
  operator: institution
  type: none
- additional_evidence:
  - content_type: application/samlmetadata+xml
    note: InCommon MDQ returns a signed SAML 2.0 EntityDescriptor for CMU's IdP.
    status: 200
    url: https://mdq.incommon.org/entities/https%3A%2F%2Flogin.cmu.edu%2Fidp%2Fshibboleth
  - note: CMU Computing Services documentation for service-provider onboarding to Web Login.
    status: 200
    url: https://www.cmu.edu/computing/services/security/identity-access/authentication/sso-provider.html
  applies_to: https://login.cmu.edu/idp/shibboleth
  description: CMU Web Login is the university's campus-wide SAML 2.0 identity provider, running Shibboleth on CMU's own host and IP space (login.cmu.edu resolves to 128.2.42.22, inside CMU's own /16). Its metadata is publicly readable at the canonical /idp/shibboleth location and it is a registered InCommon — and thereby eduGAIN — entity carrying the http://id.incommon.org/category/research-and-scholarship entity category. This is an authentication service for relying service providers, not a data API, and it is the single most unambiguously institution-operated machine-readable surface CMU publishes.
  evidence:
    content_type: application/xml
    detail: Returns an <EntityDescriptor> with entityID="https://login.cmu.edu/idp/shibboleth" and an <mdattr:EntityAttributes> block asserting the InCommon Research & Scholarship category.
    status: 200
    url: https://login.cmu.edu/idp/shibboleth
  name: CMUWebLoginShibboleth
  operator: institution
  type: saml
slug: carnegie-mellon-university-authentication
source_filename: carnegie-mellon-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-19 of every surface attributed to Carnegie Mellon University, plus\n  openapi/carnegie-mellon-university-delphi-epidata-openapi.yml and\n  openapi/carnegie-mellon-university-cert-vulnerability-notes-openapi.yml. Replaces the\n  2026-06/2026-07 file, which described the figshare OAuth 2.0 model — a vendor's auth scheme\n  recorded as CMU's.\nprovider: Carnegie Mellon University\nproviderId: carnegie-mellon-university\nsummary:\n  types:\n  - none\n  - saml\n  institution_operated_public_apis_requiring_no_auth: 2\n  oauth_surfaces_operated_by_the_institution: 0\nschemes:\n- name: DelphiEpidataPublic\n  type: none\n  operator: institution\n  applies_to: https://api.delphi.cmu.edu/epidata\n  description: >-\n    The Delphi Epidata API is public, read-only and anonymous. No key, token, header or\n    registration is required; the documentation asks only that heavy users be considerate.\n    Probed 2026-08-19\
  \ with no credential on five endpoints, all 200.\n  evidence:\n    url: https://api.delphi.cmu.edu/epidata/version\n    status: 200\n    content_type: application/json\n- name: CERTVulnerabilityNotesPublic\n  type: none\n  operator: institution\n  applies_to: https://kb.cert.org/vuls/api\n  description: >-\n    The CERT/CC Vulnerability Notes read API requires no credential. Note the failure mode: an\n    unknown identifier returns HTTP 200 with\n    {\"error\":\"Content requested either does not exist or you do not have permissions to view it!\"},\n    which conflates \"not found\" with \"not authorized\" — a client cannot distinguish a bad VU\n    number from a permission boundary.\n  evidence:\n    url: https://kb.cert.org/vuls/api/421644/\n    status: 200\n    content_type: application/json\n- name: CMUWebLoginShibboleth\n  type: saml\n  operator: institution\n  applies_to: https://login.cmu.edu/idp/shibboleth\n  description: >-\n    CMU Web Login is the university's campus-wide SAML\
  \ 2.0 identity provider, running Shibboleth\n    on CMU's own host and IP space (login.cmu.edu resolves to 128.2.42.22, inside CMU's own\n    /16). Its metadata is publicly readable at the canonical /idp/shibboleth location and it is\n    a registered InCommon — and thereby eduGAIN — entity carrying the\n    http://id.incommon.org/category/research-and-scholarship entity category. This is an\n    authentication service for relying service providers, not a data API, and it is the single\n    most unambiguously institution-operated machine-readable surface CMU publishes.\n  evidence:\n    url: https://login.cmu.edu/idp/shibboleth\n    status: 200\n    content_type: application/xml\n    detail: >-\n      Returns an <EntityDescriptor> with entityID=\"https://login.cmu.edu/idp/shibboleth\" and an\n      <mdattr:EntityAttributes> block asserting the InCommon Research & Scholarship category.\n  additional_evidence:\n  - url: https://mdq.incommon.org/entities/https%3A%2F%2Flogin.cmu.edu%2Fidp%2Fshibboleth\n\
  \    status: 200\n    content_type: application/samlmetadata+xml\n    note: InCommon MDQ returns a signed SAML 2.0 EntityDescriptor for CMU's IdP.\n  - url: https://www.cmu.edu/computing/services/security/identity-access/authentication/sso-provider.html\n    status: 200\n    note: CMU Computing Services documentation for service-provider onboarding to Web Login.\nnot_operated_by_the_institution:\n- name: figshare OAuth 2.0\n  operator: vendor\n  applies_to: https://api.figshare.com/v2\n  detail: >-\n    The 2026-06 profile recorded figshare's OAuth 2.0 authorization-code and personal-token\n    schemes as Carnegie Mellon's authentication model. They are figshare's. KiltHub\n    (kilthub.cmu.edu) is CMU's tenancy on that platform — kilthub.cmu.edu is a CNAME to\n    FIGSHARE.COM — so the data is CMU's and the auth model is not. Removed 2026-08-19.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carnegie-mellon-university/refs/heads/main/authentication/carnegie-mellon-university-authentication.yml
summary_line: none/saml · 3 schemes
tags:
- University
- Higher Education
- Education
- United States
- Private Research University
- Research
- Epidemiology
- Public Health
- Cybersecurity
- Vulnerability Disclosure
- Scholarly Publishing
- Institutional Repository
- Identity Federation
- Open Access
- Open Data
---
