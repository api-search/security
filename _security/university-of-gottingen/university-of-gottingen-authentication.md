---
api_key_in: []
api_specs:
- filename: university-of-gottingen-gdz-oai-pmh-openapi.yml
  format: yaml
  label: GDZ OAI-PMH Metadata Harvesting
  slug: gdz-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gottingen/refs/heads/main/openapi/university-of-gottingen-gdz-oai-pmh-openapi.yml
- filename: university-of-gottingen-ediss-oai-pmh-openapi.yml
  format: yaml
  label: eDiss Göttingen OAI-PMH Metadata Harvesting
  slug: ediss-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gottingen/refs/heads/main/openapi/university-of-gottingen-ediss-oai-pmh-openapi.yml
- filename: university-of-gottingen-sub-iiif-openapi.yml
  format: yaml
  label: SUB Göttingen IIIF Image and Presentation
  slug: sub-iiif
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-gottingen/refs/heads/main/openapi/university-of-gottingen-sub-iiif-openapi.yml
auth_types: []
description: 'The University of Göttingen''s public machine-readable surfaces split cleanly in two. The harvesting and image interfaces operated by SUB Göttingen are anonymous and unauthenticated — no key, no registration, no rate-limit header observed. Everything that touches people or administration sits behind institutional federated identity, and there is no self-service developer credential anywhere in the estate: the university issues no API keys to the public.'
kind: authentication
layout: security
method: generated
name: University Of Gottingen Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Göttingen declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Göttingen
provider_slug: university-of-gottingen
scheme_count: 0
schemes: []
slug: university-of-gottingen-authentication
source_filename: university-of-gottingen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: University of Göttingen\nproviderId: university-of-gottingen\ngenerated: '2026-08-30'\nmethod: generated\nx-evidence-method: probed\nsource: >-\n  Live probes of the institution's endpoints on 2026-08-30, plus the DFN-AAI/eduGAIN registration\n  record for the university's identity provider.\ndescription: >-\n  The University of Göttingen's public machine-readable surfaces split cleanly in two. The\n  harvesting and image interfaces operated by SUB Göttingen are anonymous and unauthenticated —\n  no key, no registration, no rate-limit header observed. Everything that touches people or\n  administration sits behind institutional federated identity, and there is no self-service\n  developer credential anywhere in the estate: the university issues no API keys to the public.\nmechanisms:\n- name: None (open harvesting and image delivery)\n  type: none\n  applies_to:\n  - openapi/university-of-gottingen-gdz-oai-pmh-openapi.yml\n\
  \  - openapi/university-of-gottingen-ediss-oai-pmh-openapi.yml\n  - openapi/university-of-gottingen-sub-iiif-openapi.yml\n  detail: >-\n    All confirmed 200 responses were obtained anonymously. IIIF Authentication API was not\n    advertised in the info.json profile.\n  evidence:\n  - url: https://gdz.sub.uni-goettingen.de/oai2/?verb=Identify\n    status: 200\n  - url: https://images.sub.uni-goettingen.de/iiif/image/gdz:PPN519929969:00000001/info.json\n    status: 200\n- name: SAML 2.0 / Shibboleth via DFN-AAI and eduGAIN\n  type: federated-identity\n  applies_to:\n  - Institutional web services (Stud.IP, eCampus, FlexNow, MaP, off-campus library access)\n  detail: >-\n    entityID https://shibboleth-idp.uni-goettingen.de/uni/shibboleth, registered with DFN-AAI,\n    exported to eduGAIN, Sirtfi-compliant, scope uni-goettingen.de. This is the university's own\n    identity surface and the single most substantial machine-readable thing it operates.\n  evidence:\n  - url: https://shibboleth-idp.uni-goettingen.de/uni/profile/SAML2/Redirect/SSO\n\
  \    status: 200\n- name: OAuth consumer credential (Stud.IP REST API)\n  type: oauth\n  applies_to:\n  - https://studip.uni-goettingen.de/api.php\n  detail: >-\n    The Stud.IP deployment exposes its REST API but rejects anonymous callers with\n    \"401 Unauthorized (no consumer)\". Consumer keys are issued by the institution to affiliated\n    developers; there is no public registration flow. The JSON:API surface at\n    /jsonapi.php/v1 answers with JSON:API-shaped errors, confirming the API framework is live.\n  evidence:\n  - url: https://studip.uni-goettingen.de/api.php/discovery\n    status: 401\n  - url: https://studip.uni-goettingen.de/jsonapi.php/v1/\n    status: 404\n- name: Bot challenge (not authentication)\n  type: none\n  applies_to:\n  - https://data.goettingen-research-online.de\n  - https://publications.goettingen-research-online.de\n  - https://ediss.uni-goettingen.de (HTML interface only)\n  detail: >-\n    These hosts sit behind a proof-of-work \"Site Protection: Verifying\
  \ your Request\" interstitial\n    that answers 403 to programmatic clients including a browser User-Agent. This is an\n    anti-automation measure, not an access-control scheme, and it makes the GRO.data REST and\n    OAI-PMH surfaces unreachable to harvesters. Recorded as a finding about reachability, not as\n    an authentication mechanism.\n  evidence:\n  - url: https://data.goettingen-research-online.de/api/info/version\n    status: 403\n  - url: https://data.goettingen-research-online.de/oai?verb=Identify\n    status: 403\napi_keys:\n  self_service: false\n  detail: The institution publishes no developer portal and issues no self-service API keys.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-gottingen/refs/heads/main/authentication/university-of-gottingen-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Germany
- German U15
- Public Research University
- Research Data
- Digital Library
- IIIF
- OAI-PMH
- Identity Federation
- Research Repository
---
