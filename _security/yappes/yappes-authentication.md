---
anonymous_access: false
api_key_in: []
api_specs:
- filename: yappes-openapi-generated.yml
  format: yaml
  label: Yappes API
  slug: yappes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappes/openapi/_ae-authored/yappes-openapi-generated.yml
auth_types: []
description: Authentication schemes supported by Yappes as documented.
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Yappes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yappes declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Yappes
provider_slug: yappes
scheme_count: 6
schemes:
- evidence: 'The first authentication type avaialble is HTTP Basic. If you select it, then you need to: Enter the Username . Then, Password .'
  header: Authorization
  how_to_obtain: Enter username and password in the tryout operation prompt.
  location: header
  name: HTTP Basic Authentication
  type: http-basic
- evidence: Through Header authentication, you add the authentication credentials in the headers of the API request.
  header: User-provided Header Name
  how_to_obtain: Enter Header Name and Header Value in the authentication configuration.
  location: header
  name: Header Authentication
  type: other
- authorize_url: Authorize token URL
  evidence: The third authentication type available is OAuth 1. The OAuth 1 authentication at Yappes provides a secure way to authorize user access to an API.
  header: Authorization
  how_to_obtain: Provide Consumer key, Consumer secret, Signature method, Timestamp, Nonce, Version, Realm, and token URLs.
  location: header
  name: OAuth 1 Authentication
  type: other
- evidence: The Query Parameters authentication is a simple method of authentication where the authentication credentials are passed as query parameters in the API request.
  how_to_obtain: Enter Query Parameter Name and its Value in the authentication configuration.
  location: query
  name: Query Parameters Authentication
  type: other
- authorize_url: Authentication URL (for Authorization Code grant)
  evidence: At Yappes, you can enable the OAuth 2 authentication based on Client Credentials or Authorization Code that involves Access token URL , Authentication URL and Scope.
  header: Authorization
  how_to_obtain: Select Grant Type (Client Credentials or Authorization Code), then provide Access token URL, optional Authentication URL, and Scope.
  location: header
  name: OAuth 2 Authentication
  scopes:
  - Scope (as entered)
  type: oauth2
- evidence: Yappes OAuth is a platform-managed OAuth 2.0 authentication model.
  header: Authorization
  how_to_obtain: Consumers receive per-application client credentials after subscription and obtain a Bearer token from the platform OAuth server.
  location: header
  name: Yappes OAuth
  scopes:
  - Per-endpoint scopes defined by provider
  type: other
slug: yappes-authentication
source_filename: yappes-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.yappes.com/manage_apis/related_topics/api_authentication/
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.yappes.com/manage_apis/related_topics/api_authentication/\nsources:\n- https://docs.yappes.com/manage_apis/related_topics/api_authentication/\n- https://docs.yappes.com/manage_apis/related_topics/yappes_oauth/\n- https://docs.yappes.com/admin_console/oauth2-config/\n- https://docs.yappes.com/admin_console/api-keys/\ndescription: Authentication schemes supported by Yappes as documented.\nschemes:\n- type: http-basic\n  name: HTTP Basic Authentication\n  evidence: 'The first authentication type avaialble is HTTP Basic. If you select it, then you need to: Enter the Username . Then, Password .'\n  location: header\n  header: Authorization\n  how_to_obtain: Enter username and password in the tryout operation prompt.\n- type: other\n  name: Header Authentication\n  evidence: Through Header authentication, you add the authentication credentials in the headers of the API request.\n\
  \  location: header\n  header: User-provided Header Name\n  how_to_obtain: Enter Header Name and Header Value in the authentication configuration.\n- type: other\n  name: OAuth 1 Authentication\n  evidence: The third authentication type available is OAuth 1. The OAuth 1 authentication at Yappes provides a secure way to authorize user access\n    to an API.\n  location: header\n  header: Authorization\n  authorize_url: Authorize token URL\n  how_to_obtain: Provide Consumer key, Consumer secret, Signature method, Timestamp, Nonce, Version, Realm, and token URLs.\n- type: other\n  name: Query Parameters Authentication\n  evidence: The Query Parameters authentication is a simple method of authentication where the authentication credentials are passed as query\n    parameters in the API request.\n  location: query\n  how_to_obtain: Enter Query Parameter Name and its Value in the authentication configuration.\n- type: oauth2\n  name: OAuth 2 Authentication\n  evidence: At Yappes, you can enable\
  \ the OAuth 2 authentication based on Client Credentials or Authorization Code that involves Access token\n    URL , Authentication URL and Scope.\n  location: header\n  header: Authorization\n  authorize_url: Authentication URL (for Authorization Code grant)\n  scopes:\n  - Scope (as entered)\n  how_to_obtain: Select Grant Type (Client Credentials or Authorization Code), then provide Access token URL, optional Authentication URL, and\n    Scope.\n- type: other\n  name: Yappes OAuth\n  evidence: Yappes OAuth is a platform-managed OAuth 2.0 authentication model.\n  location: header\n  header: Authorization\n  scopes:\n  - Per-endpoint scopes defined by provider\n  how_to_obtain: Consumers receive per-application client credentials after subscription and obtain a Bearer token from the platform OAuth server.\ndocs: https://docs.yappes.com/manage_apis/related_topics/api_authentication/\n"
source_yaml_url: https://artifacts.apis.io/yappes/authentication/yappes-authentication.yml
summary_line: 6 schemes
tags:
- Company
- API Management
- Unified Platform
- Developer Portal
- Analytics
---
