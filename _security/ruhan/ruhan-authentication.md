---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Ruhan Authentication
name_suffix: Authentication
oauth_flows: []
overview: RuhAN declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: RuhAN
provider_slug: ruhan
scheme_count: 0
schemes: []
slug: ruhan-authentication
source_filename: ruhan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: >-\n  Live unauthenticated probes of the two reachable RuhAN endpoints, plus a search of\n  every public RuhAN page for an authentication, API-key or OAuth reference. No OpenAPI\n  exists to derive securitySchemes from -- derive-authentication.py returned 0 profiles.\nschemes: []\nscheme_count: 0\napi_keys_issued: false\noauth2: false\nopenid_connect: false\nmutual_tls: false\nend_user_auth:\n  present: false\n  note: >-\n    /onboarding collects a user type and a primary need with a KVKK consent checkbox, but\n    it is a profile form, not a login. It states the data \"yayina cikista Supabase profil\n    kaydina tasinir\" (will be moved to a Supabase profile record at launch) -- i.e. the\n    identity store is not yet wired. /api/health confirms supabaseConfigured=false.\nendpoints:\n- endpoint: https://www.ruhan.co/api/health\n  method: GET\n  auth_required: false\n  observed_status: 200\n  note: Returns JSON to an anonymous\
  \ caller with no credential of any kind.\n- endpoint: https://www.ruhan.co/api/lead\n  methods_allowed:\n  - OPTIONS\n  - POST\n  auth_required: unknown\n  observed_status: 204\n  note: >-\n    Allow header read from an OPTIONS preflight (204). GET returns 405. Whether POST\n    demands a credential was NOT tested, because a POST here would submit a real lead\n    into the provider's system; unknown is recorded rather than guessed.\ncors:\n  access_control_allow_origin: '*'\n  observed_on: https://www.ruhan.co/\n  note: >-\n    The site root returns a wildcard CORS origin. This is a static-asset posture on\n    Vercel, not an API authorization decision, and is recorded as an observation only.\nnote: >-\n  RuhAN publishes no authentication mechanism: no API keys, no OAuth, no OIDC discovery\n  (/.well-known/openid-configuration and /.well-known/oauth-authorization-server both\n  404), and no developer key issuance anywhere on the site. Both reachable endpoints are\n  open. Server-side secrets\
  \ exist but are for an OUTBOUND integration, not an inbound one:\n  /odeme names IYZIPAY_URI, IYZIPAY_API_KEY and IYZIPAY_SECRET_KEY as environment\n  variables the server will hold to call iyzico. Those are RuhAN's credentials at a\n  payment processor, not credentials RuhAN issues to API consumers, and no value is\n  disclosed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ruhan/refs/heads/main/authentication/ruhan-authentication.yml
summary_line: 0 schemes
tags:
- Mining
- Geology
- Geophysics
- GIS
- Remote Sensing
- Mining Licensing
- Marketplace
- Turkey
---
