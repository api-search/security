---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dane-biznes-gov-pl-public-fbc-service-descriptions-controller-api-openapi.yml
  format: yaml
  label: Hurtownia danych CEIDG i Biznes.gov.pl Public Fbc Service Descriptions Controller API
  slug: dane-biznes-gov-pl-public-fbc-service-descriptions-controller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dane-biznes-gov-pl/openapi/dane-biznes-gov-pl-public-fbc-service-descriptions-controller-api-openapi.yml
- filename: dane-biznes-gov-pl-resource-api-openapi.yml
  format: yaml
  label: Hurtownia danych CEIDG i Biznes.gov.pl Resource API
  slug: dane-biznes-gov-pl-resource-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dane-biznes-gov-pl/openapi/dane-biznes-gov-pl-resource-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hurtownia danych CEIDG i Biznes.gov.pl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hurtownia danych CEIDG i Biznes.gov.pl declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hurtownia danych CEIDG i Biznes.gov.pl
provider_slug: dane-biznes-gov-pl
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Every API v3 method states "autoryzacja: TOKEN JWT w nagłówku Authorization". Example: curl -X GET "https://test-dane.biznes.gov.pl/api/ceidg/v3/firmy?nip=..." -H "Authorization: Bearer {JWT-TOKEN}".'
  header: Authorization
  in: header
  name: bearerJWT
  onboarding: Access to the Hurtownia danych requires an account; register via the access application and log in with Profil Zaufany (login.gov.pl), accepting the personal-data protection statement (dane.biznes.gov.pl home page).
  scheme: bearer
  type: http
slug: dane-biznes-gov-pl-authentication
source_filename: dane-biznes-gov-pl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: searched\nsource: https://pliki.biznes.gov.pl/akademia/20260422/Dokumentacja_dla_integratorow_API_HD_v3.7z (HD CEIDG - API v3 HD - Dokumentacja dla integratorów v1.4.pdf)\ndocs: https://akademia.biznes.gov.pl/hurtownia-danych-instrukcje-i-dokumentacja/\nschemes:\n- name: bearerJWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  header: Authorization\n  description: 'Every API v3 method states \"autoryzacja: TOKEN JWT w nagłówku Authorization\". Example: curl -X GET \"https://test-dane.biznes.gov.pl/api/ceidg/v3/firmy?nip=...\" -H \"Authorization: Bearer {JWT-TOKEN}\".'\n  onboarding: Access to the Hurtownia danych requires an account; register via the access application and log in with Profil Zaufany (login.gov.pl), accepting the personal-data protection statement (dane.biznes.gov.pl home page).\nnote: The published OpenAPI (API HD v3.json) declares no securitySchemes; the scheme is taken from the integrator PDF. Unauthenticated\
  \ GET https://dane.biznes.gov.pl/api/ceidg/v3/firmy returned 401 application/json on 2026-11-11.\n"
source_yaml_url: https://artifacts.apis.io/dane-biznes-gov-pl/authentication/dane-biznes-gov-pl-authentication.yml
summary_line: 1 scheme
tags:
- Government
- Business Registry
- Open Data
- Poland
- Companies
- Public Sector
---
