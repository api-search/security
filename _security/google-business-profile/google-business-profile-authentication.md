---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-business-profile-businessprofileperformance-locations-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Businessprofileperformance Locations API
  slug: google-business-profile-businessprofileperformance-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-businessprofileperformance-locations-api-openapi.yml
- filename: google-business-profile-mybusinessaccountmanagement-accounts-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinessaccountmanagement Accounts API
  slug: google-business-profile-mybusinessaccountmanagement-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinessaccountmanagement-accounts-api-openapi.yml
- filename: google-business-profile-mybusinessaccountmanagement-locations-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinessaccountmanagement Locations API
  slug: google-business-profile-mybusinessaccountmanagement-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinessaccountmanagement-locations-api-openapi.yml
- filename: google-business-profile-mybusinessbusinessinformation-accounts-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinessbusinessinformation Accounts API
  slug: google-business-profile-mybusinessbusinessinformation-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinessbusinessinformation-accounts-api-openapi.yml
- filename: google-business-profile-mybusinessbusinessinformation-attributes-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinessbusinessinformation Attributes API
  slug: google-business-profile-mybusinessbusinessinformation-attributes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinessbusinessinformation-attributes-api-openapi.yml
- filename: google-business-profile-mybusinessbusinessinformation-categories-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinessbusinessinformation Categories API
  slug: google-business-profile-mybusinessbusinessinformation-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinessbusinessinformation-categories-api-openapi.yml
- filename: google-business-profile-mybusinessbusinessinformation-chains-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinessbusinessinformation Chains API
  slug: google-business-profile-mybusinessbusinessinformation-chains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinessbusinessinformation-chains-api-openapi.yml
- filename: google-business-profile-mybusinessbusinessinformation-google-locations-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinessbusinessinformation Google Locations API
  slug: google-business-profile-mybusinessbusinessinformation-google-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinessbusinessinformation-google-locations-api-openapi.yml
- filename: google-business-profile-mybusinessbusinessinformation-locations-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinessbusinessinformation Locations API
  slug: google-business-profile-mybusinessbusinessinformation-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinessbusinessinformation-locations-api-openapi.yml
- filename: google-business-profile-mybusinesslodging-locations-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinesslodging Locations API
  slug: google-business-profile-mybusinesslodging-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinesslodging-locations-api-openapi.yml
- filename: google-business-profile-mybusinessnotifications-accounts-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinessnotifications Accounts API
  slug: google-business-profile-mybusinessnotifications-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinessnotifications-accounts-api-openapi.yml
- filename: google-business-profile-mybusinessplaceactions-locations-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinessplaceactions Locations API
  slug: google-business-profile-mybusinessplaceactions-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinessplaceactions-locations-api-openapi.yml
- filename: google-business-profile-mybusinessplaceactions-place-action-type-metadata-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinessplaceactions Place Action Type Metadata API
  slug: google-business-profile-mybusinessplaceactions-place-action-type-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinessplaceactions-place-action-type-metadata-api-openapi.yml
- filename: google-business-profile-mybusinessverifications-locations-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinessverifications Locations API
  slug: google-business-profile-mybusinessverifications-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinessverifications-locations-api-openapi.yml
- filename: google-business-profile-mybusinessverifications-verification-tokens-api-openapi.yml
  format: yaml
  label: Google Business Profile Business Profile Mybusinessverifications Verification Tokens API
  slug: google-business-profile-mybusinessverifications-verification-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-business-profile/openapi/google-business-profile-mybusinessverifications-verification-tokens-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Google Business Profile Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Business Profile secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Business Profile
provider_slug: google-business-profile
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: OAuth2
  sources:
  - openapi/_superseded/google-business-profile-accounts-api-openapi.yml
  type: oauth2
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/google-business-profile-businessprofileperformance-locations-api-openapi.yml
  - openapi/google-business-profile-mybusinessaccountmanagement-accounts-api-openapi.yml
  - openapi/google-business-profile-mybusinessaccountmanagement-locations-api-openapi.yml
  - openapi/google-business-profile-mybusinessbusinessinformation-accounts-api-openapi.yml
  - openapi/google-business-profile-mybusinessbusinessinformation-attributes-api-openapi.yml
  - openapi/google-business-profile-mybusinessbusinessinformation-categories-api-openapi.yml
  - openapi/google-business-profile-mybusinessbusinessinformation-chains-api-openapi.yml
  - openapi/google-business-profile-mybusinessbusinessinformation-google-locations-api-openapi.yml
  - openapi/google-business-profile-mybusinessbusinessinformation-locations-api-openapi.yml
  - openapi/google-business-profile-mybusinesslodging-locations-api-openapi.yml
  - openapi/google-business-profile-mybusinessnotifications-accounts-api-openapi.yml
  - openapi/google-business-profile-mybusinessplaceactions-locations-api-openapi.yml
  - openapi/google-business-profile-mybusinessplaceactions-place-action-type-metadata-api-openapi.yml
  - openapi/google-business-profile-mybusinessverifications-locations-api-openapi.yml
  - openapi/google-business-profile-mybusinessverifications-verification-tokens-api-openapi.yml
  type: apiKey
slug: google-business-profile-authentication
source_filename: google-business-profile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/_superseded/google-business-profile-accounts-api-openapi.yml, openapi/google-business-profile-businessprofileperformance-locations-api-openapi.yml,\n  openapi/google-business-profile-mybusinessaccountmanagement-accounts-api-openapi.yml, openapi/google-business-profile-mybusinessaccountmanagement-locations-api-openapi.yml,\n  openapi/google-business-profile-mybusinessbusinessinformation-accounts-api-openapi.yml, openapi/google-business-profile-mybusinessbusinessinformation-attributes-api-openapi.yml,\n  openapi/google-business-profile-mybusinessbusinessinformation-categories-api-openapi.yml,\n  openapi/google-business-profile-mybusinessbusinessinformation-chains-api-openapi.yml, openapi/google-business-profile-mybusinessbusinessinformation-google-locations-api-openapi.yml,\n  openapi/google-business-profile-mybusinessbusinessinformation-locations-api-openapi.yml, openapi/google-business-profile-mybusinesslodging-locations-api-openapi.yml,\n\
  \  openapi/google-business-profile-mybusinessnotifications-accounts-api-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  sources:\n  - openapi/_superseded/google-business-profile-accounts-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/google-business-profile-businessprofileperformance-locations-api-openapi.yml\n  - openapi/google-business-profile-mybusinessaccountmanagement-accounts-api-openapi.yml\n  - openapi/google-business-profile-mybusinessaccountmanagement-locations-api-openapi.yml\n  - openapi/google-business-profile-mybusinessbusinessinformation-accounts-api-openapi.yml\n\
  \  - openapi/google-business-profile-mybusinessbusinessinformation-attributes-api-openapi.yml\n  - openapi/google-business-profile-mybusinessbusinessinformation-categories-api-openapi.yml\n  - openapi/google-business-profile-mybusinessbusinessinformation-chains-api-openapi.yml\n  - openapi/google-business-profile-mybusinessbusinessinformation-google-locations-api-openapi.yml\n  - openapi/google-business-profile-mybusinessbusinessinformation-locations-api-openapi.yml\n  - openapi/google-business-profile-mybusinesslodging-locations-api-openapi.yml\n  - openapi/google-business-profile-mybusinessnotifications-accounts-api-openapi.yml\n  - openapi/google-business-profile-mybusinessplaceactions-locations-api-openapi.yml\n  - openapi/google-business-profile-mybusinessplaceactions-place-action-type-metadata-api-openapi.yml\n  - openapi/google-business-profile-mybusinessverifications-locations-api-openapi.yml\n  - openapi/google-business-profile-mybusinessverifications-verification-tokens-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-business-profile/authentication/google-business-profile-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Business Profiles
- Google
- Local Business
- Location
- Reviews
---
