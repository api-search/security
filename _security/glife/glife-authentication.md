---
api_key_in: []
auth_types:
- token
description: ''
kind: authentication
layout: security
method: derived
name: Glife Authentication
name_suffix: Authentication
oauth_flows: []
overview: Glife secures its APIs with token across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Glife
provider_slug: glife
scheme_count: 0
schemes: []
slug: glife-authentication
source_filename: glife-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: graphql/glife-schema.graphql\ndocs: null\nsummary:\n  types:\n  - token\n  model: GraphQL mutation-based credential login returning a bearer token (JWT-style)\n    + refresh token; token presented on subsequent requests. No OpenAPI securitySchemes\n    (GraphQL API).\n  transport: Authorization header bearer token (derived; single GraphQL POST endpoint)\nlogin_operations:\n- mutation: login\n  args:\n  - username\n  - password\n  returns: LoginResponse{token,refreshToken,user}\n  audience: internal/back-office\n- mutation: loginEcommerce\n  args:\n  - email\n  - mobileCode\n  - mobileNumber\n  - mode\n  - password\n  returns: LoginResponse{token,refreshToken,user}\n  audience: ecommerce customer\n- mutation: loginDriver\n  returns: LoginResponse\n  audience: driver app\n- mutation: registerCustomer\n  args:\n  - email\n  - mobileCode\n  - mobileNumber\n  - firstName\n  - lastName\n  - companyName\n  - outletName\n  returns:\
  \ RegisterResponse\n- mutation: registerEcommerceCustomer\n  args:\n  - email\n  - mobileCode\n  - mobileNumber\n  - fullName\n  - password\n  - companyName\n  returns: RegisterResponse\n- mutation: forgotPassword\n  returns: —\n- mutation: resetPassword\n  returns: —\n- mutation: generateOTPVerification\n  returns: —\n  note: SMS/email OTP issuance\n- mutation: verifyOTPVerification\n  args:\n  - code\n  returns: CommonResponse\n  note: OTP verification step\nnotes: Derived from live GraphQL introspection. LoginResponse exposes token + refreshToken;\n  two-factor via OTP mutations. Bearer transport inferred from standard GraphQL/JWT\n  practice — not published in a securityScheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glife/refs/heads/main/authentication/glife-authentication.yml
summary_line: token · 0 schemes
tags:
- Company
- Food Tech
- Grocery
- Supply Chain
- E-Commerce
- GraphQL
- Southeast Asia
- AgTech
- Logistics
---
