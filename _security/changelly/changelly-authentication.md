---
anonymous_access: false
api_key_in: []
api_specs:
- filename: changelly-openapi-generated.yml
  format: yaml
  label: Changelly API
  slug: changelly-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/changelly/openapi/_ae-authored/changelly-openapi-generated.yml
auth_types: []
description: 'All requests must contain the following headers: Header Description X-Api-Key Your API key (SHA256 from public key). X-Api-Signature The query''s serialized body signed by your private key according to the RSA-SHA256 method.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Changelly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Changelly declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Changelly
provider_slug: changelly
scheme_count: 2
schemes:
- evidence: 'All requests must contain the following headers: Header Description X-Api-Key Your API key (SHA256 from public key). X-Api-Signature The query''s serialized body signed by your private key according to the RSA-SHA256 method.'
  header: X-Api-Key
  location: header
  name: X-Api-Key
  type: apiKey
- evidence: 'All requests must contain the following headers: Header Description X-Api-Key Your API key (SHA256 from public key). X-Api-Signature The query''s serialized body signed by your private key according to the RSA-SHA256 method.'
  header: X-Api-Signature
  location: header
  name: X-Api-Signature
  type: apiKey
slug: changelly-authentication
source_filename: changelly-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.changelly.com/development/authentication
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.changelly.com/development/authentication\nsources:\n- https://docs.changelly.com/development/authentication\n- https://docs.changelly.com/development/generate-keys\ndescription: 'All requests must contain the following headers: Header Description X-Api-Key Your API key (SHA256 from public key). X-Api-Signature\n  The query''s serialized body signed by your private key according to the RSA-SHA256 method.'\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: 'All requests must contain the following headers: Header Description X-Api-Key Your API key (SHA256 from public key). X-Api-Signature\n    The query''s serialized body signed by your private key according to the RSA-SHA256 method.'\n  location: header\n  header: X-Api-Key\n- type: apiKey\n  name: X-Api-Signature\n  evidence: 'All requests must contain the following headers: Header Description X-Api-Key Your API\
  \ key (SHA256 from public key). X-Api-Signature\n    The query''s serialized body signed by your private key according to the RSA-SHA256 method.'\n  location: header\n  header: X-Api-Signature\nnote: No OAuth2 or other authentication methods are documented on the provided pages.\ndocs: https://docs.changelly.com/development/authentication\n"
source_yaml_url: https://artifacts.apis.io/changelly/authentication/changelly-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cryptocurrency
- Exchange
- Fintech
---
