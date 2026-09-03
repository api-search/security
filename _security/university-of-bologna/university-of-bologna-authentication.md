---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: University Of Bologna Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Bologna declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Bologna
provider_slug: university-of-bologna
scheme_count: 0
schemes: []
slug: university-of-bologna-authentication
source_filename: university-of-bologna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: University of Bologna — authentication surfaces\nslug: university-of-bologna\ngenerated: '2026-09-01'\nmethod: probed\nsource: https://www.unibo.it/en\nnote: >-\n  How the University of Bologna's machine surfaces authenticate, recorded from live\n  unauthenticated probes on 2026-09-01. This artifact exists mainly to record what is NOT\n  callable: three REST APIs sit on institution or institution-branded hosts and all three\n  refuse anonymous callers. They are documented here rather than counted as public APIs. No\n  credentials of any kind were used or attempted; every response below is what a member of\n  the public receives.\nsurfaces:\n  - name: CKAN Action API (dati.unibo.it)\n    x-operator: institution\n    auth: none\n    self_service_keys: false\n    detail: >-\n      Anonymous read. https://dati.unibo.it/api/3/action/package_list returned 200\n      application/json with success:true, and status_show returned ckan_version 2.6.9. Write\n      operations\
  \ in CKAN require an API key issued from a portal user account; no public\n      signup or key-issuance flow was found on this deployment. The only unauthenticated,\n      genuinely callable API the university operates.\n    evidence:\n      - url: https://dati.unibo.it/api/3/action/package_list\n        status: 200\n      - url: https://dati.unibo.it/api/3/action/status_show\n        status: 200\n  - name: AlmaDL OAI-PMH providers (AMS Acta, AMS Dottorato, AMS Laurea, AlmaDL Journals)\n    x-operator: institution\n    auth: none\n    self_service_keys: false\n    detail: >-\n      All four OAI-PMH 2.0 endpoints answer unauthenticated GET requests for Identify,\n      ListMetadataFormats, ListSets and ListRecords. OAI-PMH has no authentication layer by\n      design; these are open harvesting surfaces.\n    evidence:\n      - url: https://amsacta.unibo.it/cgi/oai2?verb=Identify\n        status: 200\n      - url: https://amsdottorato.unibo.it/cgi/oai2?verb=Identify\n        status: 200\n\
  \      - url: https://amslaurea.unibo.it/cgi/oai2?verb=Identify\n        status: 200\n      - url: https://journals.unibo.it/index.php/index/oai?verb=Identify\n        status: 200\n  - name: AlmaDL Journals OJS REST API v1\n    x-operator: institution\n    auth: token\n    self_service_keys: false\n    callable_anonymously: false\n    detail: >-\n      The Open Journal Systems REST API is present on the institution's own host and closed.\n      https://journals.unibo.it/index.php/ijhb/api/v1/issues returns 403 application/json\n      {\"error\":\"api.403.unauthorized\",\"errorMessage\":\"You are not authorized to access the\n      requested resource.\"}. The site-wide https://journals.unibo.it/api/v1/contexts returns\n      500 with an empty body. OJS API tokens are issued from an editorial user profile inside\n      each journal; there is no public developer registration.\n    evidence:\n      - url: https://journals.unibo.it/index.php/ijhb/api/v1/issues\n        status: 403\n      -\
  \ url: https://journals.unibo.it/api/v1/contexts\n        status: 500\n  - name: Virtuale (Moodle) Web Services REST API\n    x-operator: institution\n    auth: token\n    self_service_keys: false\n    callable_anonymously: false\n    detail: >-\n      https://virtuale.unibo.it/webservice/rest/server.php returns 200 application/xml with\n      <EXCEPTION class=\"core\\exception\\moodle_exception\"><ERRORCODE>invalidtoken</ERRORCODE>\n      <MESSAGE>Token non valido - il token non è stato trovato</MESSAGE>. A live, correctly\n      rejecting endpoint — not a soft 404 — but tokens are issued by the university to\n      approved integrations, not self-service, so this is not a public API.\n    evidence:\n      - url: https://virtuale.unibo.it/webservice/rest/server.php\n        status: 200\n  - name: Virtuale (Moodle) LTI 1.3 platform\n    x-operator: institution\n    auth: oauth2\n    flow: client_credentials\n    self_service_keys: false\n    detail: >-\n      The LTI 1.3 platform surface\
  \ is partly public by design: the JWKS at\n      https://virtuale.unibo.it/mod/lti/certs.php is served unauthenticated (200\n      application/json, RS256 key kid a0f8811debf999e8089e) because tool providers must fetch\n      it to verify the platform's signatures. The paired token endpoint\n      https://virtuale.unibo.it/mod/lti/token.php implements OAuth2 client credentials with a\n      signed JWT assertion and returns 400 {\"error\":\"invalid_request\"} to an empty request.\n      Client registration is per-tool, arranged with the university.\n    evidence:\n      - url: https://virtuale.unibo.it/mod/lti/certs.php\n        status: 200\n      - url: https://virtuale.unibo.it/mod/lti/token.php\n        status: 400\n  - name: IRIS DSpace-CRIS REST API (cris.unibo.it)\n    x-operator: tenant\n    auth: basic\n    self_service_keys: false\n    callable_anonymously: false\n    detail: >-\n      https://cris.unibo.it/rest/api returns 401 \"HTTP Status 401 - Invalid basic\n      authentication\
  \ token\"; https://cris.unibo.it/server/api returns the Angular shell\n      (soft-200, not an API root). The host CNAMEs to unibo.prod.iris.cineca.it, so both the\n      software and the auth design are CINECA's. Only the OAI-PMH provider on this host is\n      open.\n    evidence:\n      - url: https://cris.unibo.it/rest/api\n        status: 401\n      - url: https://cris.unibo.it/server/api\n        status: 200\n  - name: Shibboleth Identity Provider (shib.unibo.it)\n    x-operator: federation\n    auth: saml2\n    self_service_keys: false\n    detail: >-\n      The IdP metadata document itself is published unauthenticated — that is the point of\n      federation metadata — at https://shib.unibo.it/idp/shibboleth (200 application/xml,\n      7,625 bytes). It advertises SAML 2.0 SingleSignOnService endpoints for HTTP-POST,\n      HTTP-POST-SimpleSign and HTTP-Redirect. Authentication itself is interactive SSO for\n      institutional accounts and is not a programmable surface. A second,\
  \ ADFS-based SP\n      (http://idp.unibo.it/adfs/services/trust) fronts institutional web applications; e.g.\n      https://site.unibo.it/ redirects into an ADFS SAMLRequest.\n    evidence:\n      - url: https://shib.unibo.it/idp/shibboleth\n        status: 200\n      - url: https://md.idem.garr.it/metadata/idem-metadata-sha256.xml\n        status: 200\nabsent:\n  - developer_portal: >-\n      No developer portal, no API key signup, no self-service onboarding on any unibo.it host.\n      api.unibo.it does not resolve.\n  - api_terms: >-\n      No API-specific terms of service or acceptable-use policy was found for any surface. The\n      institutional privacy and legal notes at\n      https://www.unibo.it/en/university/privacy-policy-and-legal-notes (200) are the closest\n      published document and do not address API use.\n  - rate_limits: >-\n      No published rate limits for any surface. During this run dati.unibo.it stopped\n      answering our client entirely after two successful\
  \ requests — TCP 443 still accepted a\n      connection but no HTTP response returned within 60s — which is consistent with an\n      undocumented WAF or rate-limit reaction rather than an outage.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-bologna/refs/heads/main/authentication/university-of-bologna-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Italy
- Europe
- Research
- Research Repository
- Open Data
- Open Access
- Library
- OAI-PMH
- Identity Federation
- Scholarly Publishing
- Learning Management
---
