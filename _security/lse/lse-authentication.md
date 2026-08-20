---
api_key_in: []
api_specs:
- filename: lse-moodle-lti-platform-openapi.yml
  format: yaml
  label: LSE Moodle LTI 1.3 Platform
  slug: moodle-lti-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lse/refs/heads/main/openapi/lse-moodle-lti-platform-openapi.yml
auth_types: []
description: How authentication actually works across LSE's programmable surfaces, split by who operates each one. LSE operates its own SAML2 identity provider and its own LTI 1.3 platform; everything else affiliated with the institution authenticates against a vendor's platform under an LSE tenancy.
kind: authentication
layout: security
method: probed
name: Lse Authentication
name_suffix: Authentication
oauth_flows: []
overview: London School of Economics and Political Science declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: London School of Economics and Political Science
provider_slug: lse
scheme_count: 0
schemes: []
slug: lse-authentication
source_filename: lse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: London School of Economics and Political Science — authentication surfaces\ndescription: >-\n  How authentication actually works across LSE's programmable surfaces, split by who\n  operates each one. LSE operates its own SAML2 identity provider and its own LTI 1.3\n  platform; everything else affiliated with the institution authenticates against a\n  vendor's platform under an LSE tenancy.\ngenerated: '2026-08-19'\nmethod: probed\nsource: live HTTP probes and UK Access Management Federation metadata, 2026-08-19\nauthentication:\n  - name: LSE Shibboleth Identity Provider (SAML2)\n    x-operator: institution\n    type: SAML2 / Shibboleth\n    entity_id: https://lse.ac.uk/idp\n    metadata_url: https://gate.library.lse.ac.uk/idp/shibboleth\n    metadata_status: 200\n    metadata_content_type: application/xml;charset=UTF-8\n    federation: UK Access Management Federation (UKAMF)\n    federation_metadata: http://metadata.ukfederation.org.uk/ukfederation-metadata.xml\n\
  \    display_name: LSE - London School of Economics and Political Science\n    scope: lse.ac.uk\n    protocols:\n      - urn:oasis:names:tc:SAML:2.0:protocol\n    bindings:\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n    endpoints:\n      - url: https://gate.library.lse.ac.uk/idp/profile/SAML2/Redirect/SSO\n      - url: https://gate.library.lse.ac.uk/idp/profile/SAML2/POST/SSO\n      - url: https://gate.library.lse.ac.uk:8443/idp/profile/SAML2/SOAP/ArtifactResolution\n    defects:\n      - issue: >-\n          The POST-SimpleSign SSO Location published in LSE's federation metadata is\n          https://gate.library.lse.ac.uk.lse.ac.uk/idp/profile/SAML2/POST-SimpleSign/SSO\n          — a doubled domain. The host does not resolve (NXDOMAIN, verified\n          2026-08-19). A relying party that selects the SimpleSign binding from LSE's\n          published\
  \ metadata cannot reach it.\n        severity: medium\n        verified: '2026-08-19'\n    note: >-\n      A second LSE entity is registered in UKAMF at\n      https://idp.lse.ac.uk/idp/shibboleth with the display name\n      \"LSE - London School of Economics and Political Science - Test IdP - DO NOT USE\".\n      It does not resolve. It is a non-production entity and is deliberately NOT\n      recorded as a surface in apis.yml.\n  - name: LSE Moodle SAML2 Service Provider\n    x-operator: institution\n    type: SAML2 SP\n    entity_id: https://moodle.lse.ac.uk/auth/saml2/sp/metadata.php\n    metadata_url: https://moodle.lse.ac.uk/auth/saml2/sp/metadata.php\n    metadata_status: 200\n    authn_requests_signed: true\n    want_assertions_signed: false\n    technical_contact: lti.support@lse.ac.uk\n    note: >-\n      The VLE is a service provider against the LSE IdP. WantAssertionsSigned is\n      false, which is common for Moodle's saml2 plugin but is a weaker posture than\n      requiring\
  \ signed assertions.\n  - name: LSE Moodle LTI 1.3 platform (OAuth 2.0 / OIDC)\n    x-operator: institution\n    type: OAuth 2.0 client credentials with JWT bearer client assertion (RFC 7523)\n    issuer: https://moodle.lse.ac.uk\n    jwks_uri: https://moodle.lse.ac.uk/mod/lti/certs.php\n    jwks_status: 200\n    token_endpoint: https://moodle.lse.ac.uk/mod/lti/token.php\n    authorization_endpoint: https://moodle.lse.ac.uk/mod/lti/auth.php\n    keys_observed: 1 RSA RS256 signing key (kid fc7fb5f6ed67a729c4d6)\n    note: >-\n      Registration is closed — a tool must be registered by LSE before it can obtain\n      a token. There is no public self-service registration and no published\n      .well-known discovery document for this issuer.\n  - name: LSE Moodle Web Services\n    x-operator: institution\n    type: Bearer token (Moodle wstoken)\n    token_endpoint: https://moodle.lse.ac.uk/login/token.php\n    service_endpoint: https://moodle.lse.ac.uk/webservice/rest/server.php\n    status:\
  \ live, credentialed\n    note: >-\n      Enabled and reachable, but issuing a token requires LSE credentials and an\n      enabled external service. Not a public API.\n  - name: Vendor-platform authentication under LSE tenancy\n    x-operator: tenant\n    covers:\n      - Ex Libris Alma/Primo VE (librarysearch.lse.ac.uk, vid=44LSE_INST)\n      - EPrints Services (researchonline.lse.ac.uk)\n      - Quartex (digital.library.lse.ac.uk)\n      - Epexio (archives.lse.ac.uk)\n    note: >-\n      Authentication for these is defined by the vendor, configured by LSE. Credit\n      for the auth contract belongs to the vendor's own catalog entry, not to LSE.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lse/refs/heads/main/authentication/lse-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Social Sciences
- Identity Federation
- Learning Management
- Research Repository
- Library
- Open Research
- OAI-PMH
- SAML
- LTI
- IIIF
---
