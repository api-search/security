---
api_key_in: []
api_specs:
- filename: kau-open-data-api-openapi.yml
  format: yaml
  label: KAU Open Data API
  slug: open-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kau/refs/heads/main/openapi/kau-open-data-api-openapi.yml
auth_types: []
description: 'Authentication posture across every King Abdulaziz University surface reachable from the open internet. The shape is unusual for this cohort and worth stating plainly: the one API KAU operates itself is completely open and requires nothing, while everything that is gated is gated by a vendor platform in front of KAU''s own identity provider. There is no developer-facing credential of any kind — no API key, no client registration, no OAuth application, no self-service onboarding — anywhere in KAU''s public footprint.'
kind: authentication
layout: security
method: probed
name: Kau Authentication
name_suffix: Authentication
oauth_flows: []
overview: King Abdulaziz University declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: King Abdulaziz University
provider_slug: kau
scheme_count: 4
schemes:
- applies_to: https://opendata.kau.edu.sa/api/StudentsData
  caveat: Open in contract, restricted in reach. The host refused connections from two independent network egresses during this run while KAU's CloudFront-fronted www host answered normally, which reads as a geographic restriction on KAU's self-hosted estate. An unauthenticated API that only answers from inside one country is, in practice, access-controlled by network rather than by credential.
  confidence: high
  description: KAU's Open Data API takes no credential. All eight invocations KAU publishes on https://www.kau.edu.sa/page/open-data are plain GETs with query parameters and no authentication element, and the archived 2025-04-17 capture returned a full 1,886 record payload with no authorization header sent. There is no key to request, no registration step and no quota published.
  name: None — open data web service
  type: none
  x-operator: institution
- binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
  confidence: high
  description: The institutional identity provider behind every gated KAU service. Evidenced by a live, signed AuthnRequest addressed to it during this run; see identity-federation/kau-identity-federation.yml and identity-federation/kau-lms-saml-authnrequest.xml.
  developer_accessible: false
  developer_accessible_basis: This is an institutional login for enrolled students and staff, not a developer authorization server. No metadata is published, no relying party can register, and KAU belongs to neither the Maeen national federation nor eduGAIN — so no external party can federate with it even in principle.
  idp_endpoint: https://iam.kau.edu.sa/oamfed/idp/samlv20
  name: KAU SAML 2.0 single sign-on
  related_endpoints:
  - note: Unreachable on 443 from this run's egresses; DNS resolves to 192.162.72.15.
    role: Institutional SSO portal, linked from KAU's own Open Data page.
    status: 0
    url: https://sso.kau.edu.sa/
  - note: Unreachable from this run. Recorded in the 2026-06-03 profile as KAU's federation endpoint; the actual SAML 2.0 protocol endpoint is /oamfed/idp/samlv20, corrected here from live evidence.
    role: Oracle Access Manager federated login entry point.
    status: 0
    url: https://iam.kau.edu.sa/oamsso-bin/login-fed.pl
  signature_algorithm: http://www.w3.org/2001/04/xmldsig-more#rsa-sha256
  software: Oracle Access Manager Federation
  type: saml
  x-operator: institution
- applies_to: https://lms.kau.edu.sa/learn/api/public/v1/
  authorization_endpoint: https://lms.kau.edu.sa/learn/api/public/v1/oauth2/authorizationcode
  confidence: moderate
  description: Blackboard Learn's standard REST authorization surface, provisioned and answering on KAU's tenancy. /learn/api/public/v1/courses returns a JSON 401 "API request is not authenticated" rather than a 404, and the authorizationcode endpoint returns a 400 rather than a 404, so the OAuth surface is genuinely deployed here.
  developer_accessible: false
  developer_accessible_basis: Application registration for a Blackboard Learn tenancy happens in Blackboard's own developer portal and then requires the institution's administrator to authorize the application against this tenancy. KAU publishes no developer onboarding path, no application-approval process and no contact for one. The credential is Blackboard's to issue and KAU's to approve, and KAU documents neither.
  name: Blackboard Learn REST — OAuth 2.0
  operator: Blackboard (Anthology)
  token_endpoint: https://lms.kau.edu.sa/learn/api/public/v1/oauth2/token
  type: oauth2
  unauthenticated_exceptions:
  - note: Product version only; the sole endpoint on the tenancy that answers without a token.
    status: 200
    url: https://lms.kau.edu.sa/learn/api/public/v1/system/version
  x-operator: tenant
- applies_to: https://kauj.researchcommons.org/do/oai/
  confidence: high
  description: KAU's journal metadata is harvestable anonymously over OAI-PMH 2.0 with no credential — Identify and ListSets both returned 200. Genuinely open, and genuinely not KAU's implementation.
  name: None — OAI-PMH anonymous harvesting
  operator: Elsevier (Digital Commons / bepress)
  type: none
  x-operator: tenant
slug: kau-authentication
source_filename: kau-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Evangelist Authentication\nspecificationVersion: '0.1'\nprovider: King Abdulaziz University\nproviderId: kau\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes on 2026-09-01: https://lms.kau.edu.sa/ (200, redirects to SAML login),\n  https://lms.kau.edu.sa/learn/api/public/v1/system/version (200, unauthenticated),\n  https://lms.kau.edu.sa/learn/api/public/v1/courses (401),\n  https://lms.kau.edu.sa/learn/api/public/v1/lti/domainConfigs (401),\n  https://lms.kau.edu.sa/learn/api/public/v1/oauth2/authorizationcode (400),\n  https://lms.kau.edu.sa/auth-saml/saml/metadata?apId=_7123_1 (200),\n  https://kauj.researchcommons.org/do/oai/?verb=Identify (200, anonymous),\n  https://sso.kau.edu.sa/ and https://iam.kau.edu.sa/oamsso-bin/login-fed.pl (both\n  unreachable on 443 from two network egresses). The open data API's authentication\n  posture is read from KAU's own published URLs and the archived 200 response, not from\n  a live call.\ndescription:\
  \ >-\n  Authentication posture across every King Abdulaziz University surface reachable from\n  the open internet. The shape is unusual for this cohort and worth stating plainly: the\n  one API KAU operates itself is completely open and requires nothing, while everything\n  that is gated is gated by a vendor platform in front of KAU's own identity provider.\n  There is no developer-facing credential of any kind — no API key, no client\n  registration, no OAuth application, no self-service onboarding — anywhere in KAU's\n  public footprint.\n\nschemes:\n  - name: None — open data web service\n    type: none\n    x-operator: institution\n    applies_to: https://opendata.kau.edu.sa/api/StudentsData\n    description: >-\n      KAU's Open Data API takes no credential. All eight invocations KAU publishes on\n      https://www.kau.edu.sa/page/open-data are plain GETs with query parameters and no\n      authentication element, and the archived 2025-04-17 capture returned a full 1,886\n      record\
  \ payload with no authorization header sent. There is no key to request, no\n      registration step and no quota published.\n    confidence: high\n    caveat: >-\n      Open in contract, restricted in reach. The host refused connections from two\n      independent network egresses during this run while KAU's CloudFront-fronted\n      www host answered normally, which reads as a geographic restriction on KAU's\n      self-hosted estate. An unauthenticated API that only answers from inside one\n      country is, in practice, access-controlled by network rather than by credential.\n\n  - name: KAU SAML 2.0 single sign-on\n    type: saml\n    x-operator: institution\n    idp_endpoint: https://iam.kau.edu.sa/oamfed/idp/samlv20\n    software: Oracle Access Manager Federation\n    binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n    signature_algorithm: http://www.w3.org/2001/04/xmldsig-more#rsa-sha256\n    description: >-\n      The institutional identity provider behind every gated\
  \ KAU service. Evidenced by a\n      live, signed AuthnRequest addressed to it during this run; see\n      identity-federation/kau-identity-federation.yml and\n      identity-federation/kau-lms-saml-authnrequest.xml.\n    confidence: high\n    developer_accessible: false\n    developer_accessible_basis: >-\n      This is an institutional login for enrolled students and staff, not a developer\n      authorization server. No metadata is published, no relying party can register, and\n      KAU belongs to neither the Maeen national federation nor eduGAIN — so no external\n      party can federate with it even in principle.\n    related_endpoints:\n      - url: https://sso.kau.edu.sa/\n        role: Institutional SSO portal, linked from KAU's own Open Data page.\n        status: 0\n        note: Unreachable on 443 from this run's egresses; DNS resolves to 192.162.72.15.\n      - url: https://iam.kau.edu.sa/oamsso-bin/login-fed.pl\n        role: Oracle Access Manager federated login entry point.\n\
  \        status: 0\n        note: >-\n          Unreachable from this run. Recorded in the 2026-06-03 profile as KAU's\n          federation endpoint; the actual SAML 2.0 protocol endpoint is\n          /oamfed/idp/samlv20, corrected here from live evidence.\n\n  - name: Blackboard Learn REST — OAuth 2.0\n    type: oauth2\n    x-operator: tenant\n    operator: Blackboard (Anthology)\n    applies_to: https://lms.kau.edu.sa/learn/api/public/v1/\n    token_endpoint: https://lms.kau.edu.sa/learn/api/public/v1/oauth2/token\n    authorization_endpoint: https://lms.kau.edu.sa/learn/api/public/v1/oauth2/authorizationcode\n    description: >-\n      Blackboard Learn's standard REST authorization surface, provisioned and answering\n      on KAU's tenancy. /learn/api/public/v1/courses returns a JSON 401 \"API request is\n      not authenticated\" rather than a 404, and the authorizationcode endpoint returns a\n      400 rather than a 404, so the OAuth surface is genuinely deployed here.\n    confidence:\
  \ moderate\n    developer_accessible: false\n    developer_accessible_basis: >-\n      Application registration for a Blackboard Learn tenancy happens in Blackboard's\n      own developer portal and then requires the institution's administrator to\n      authorize the application against this tenancy. KAU publishes no developer\n      onboarding path, no application-approval process and no contact for one. The\n      credential is Blackboard's to issue and KAU's to approve, and KAU documents\n      neither.\n    unauthenticated_exceptions:\n      - url: https://lms.kau.edu.sa/learn/api/public/v1/system/version\n        status: 200\n        note: Product version only; the sole endpoint on the tenancy that answers without a token.\n\n  - name: None — OAI-PMH anonymous harvesting\n    type: none\n    x-operator: tenant\n    operator: Elsevier (Digital Commons / bepress)\n    applies_to: https://kauj.researchcommons.org/do/oai/\n    description: >-\n      KAU's journal metadata is harvestable\
  \ anonymously over OAI-PMH 2.0 with no\n      credential — Identify and ListSets both returned 200. Genuinely open, and\n      genuinely not KAU's implementation.\n    confidence: high\n\ndeveloper_credentials:\n  available: false\n  basis: >-\n    No API key, client registration, developer account, application form or credential\n    request path exists anywhere in KAU's public footprint. www.kau.edu.sa returns 404\n    for /robots.txt, /sitemap.xml, /.well-known/security.txt, /apis.json and\n    /openapi.json, there is no developer portal, and there is no official KAU GitHub\n    organisation (GitHub org lookup 404; org-scoped search returned 0 results). The Open\n    Data API needs no credential; everything else needs an enrolled institutional\n    identity that cannot be obtained from outside the university.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kau/refs/heads/main/authentication/kau-authentication.yml
summary_line: 4 schemes
tags:
- University
- Higher Education
- Education
- Research
- Open Data
- Research Repository
- Identity Federation
- Learning Management
- Saudi Arabia
- Middle East
---
