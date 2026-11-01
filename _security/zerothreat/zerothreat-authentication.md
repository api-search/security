---
anonymous_access: false
api_key_in: []
auth_types: []
description: ZeroThreat supports testing of JWT and Basic authentication schemes.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Zerothreat Authentication
name_suffix: Authentication
oauth_flows: []
overview: ZeroThreat declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ZeroThreat
provider_slug: zerothreat
scheme_count: 2
schemes:
- evidence: JWT Authentication Verify signature integrity, claim validation, and expiration handling to ensure secure token management.
  header: Authorization
  location: header
  name: JWT Authentication
  type: jwt
- evidence: Role-Based Access Control Easily define and enforce access policies based on user roles and responsibilities with basic auth test.
  header: Authorization
  location: header
  name: Basic Auth Test
  type: http-basic
slug: zerothreat-authentication
source_filename: zerothreat-authentication.yml
source_heading: Authentication Profile
source_url: https://zerothreat.ai/authentication-and-authorization
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://zerothreat.ai/authentication-and-authorization\nsources:\n- https://zerothreat.ai/authentication-and-authorization\n- https://zerothreat.ai/blog/explaining-broken-authentication-with-tips-to-prevent-it\n- https://zerothreat.ai/blog/ultimate-guide-to-token-based-authentication\n- https://zerothreat.ai/blog/what-is-multi-factor-authentication\ndescription: ZeroThreat supports testing of JWT and Basic authentication schemes.\nschemes:\n- type: jwt\n  name: JWT Authentication\n  evidence: JWT Authentication Verify signature integrity, claim validation, and expiration handling to ensure secure token management.\n  location: header\n  header: Authorization\n- type: http-basic\n  name: Basic Auth Test\n  evidence: Role-Based Access Control Easily define and enforce access policies based on user roles and responsibilities with basic auth test.\n  location: header\n  header: Authorization\n\
  docs: https://zerothreat.ai/authentication-and-authorization\n"
source_yaml_url: https://artifacts.apis.io/zerothreat/authentication/zerothreat-authentication.yml
summary_line: 2 schemes
tags:
- Pentesting
- Web Application Security
- API Security
- DevOps
- Enterprise Security
- Compliance
---
