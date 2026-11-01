---
anonymous_access: false
api_key_in: []
api_specs:
- filename: conversion-audiences-api-openapi.yml
  format: yaml
  label: Conversion Audiences API
  slug: conversion-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-audiences-api-openapi.yml
- filename: conversion-campaigns-api-openapi.yml
  format: yaml
  label: Conversion Campaigns API
  slug: conversion-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-campaigns-api-openapi.yml
- filename: conversion-contacts-api-openapi.yml
  format: yaml
  label: Conversion Contacts API
  slug: conversion-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-contacts-api-openapi.yml
- filename: conversion-custom-objects-api-openapi.yml
  format: yaml
  label: Conversion Custom Objects API
  slug: conversion-custom-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-custom-objects-api-openapi.yml
- filename: conversion-events-api-openapi.yml
  format: yaml
  label: Conversion Events API
  slug: conversion-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-events-api-openapi.yml
- filename: conversion-exports-api-openapi.yml
  format: yaml
  label: Conversion Exports API
  slug: conversion-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-exports-api-openapi.yml
- filename: conversion-fields-api-openapi.yml
  format: yaml
  label: Conversion Fields API
  slug: conversion-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-fields-api-openapi.yml
- filename: conversion-forms-api-openapi.yml
  format: yaml
  label: Conversion Forms API
  slug: conversion-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-forms-api-openapi.yml
- filename: conversion-full-delete-api-openapi.yml
  format: yaml
  label: Conversion Full Delete API
  slug: conversion-full-delete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-full-delete-api-openapi.yml
- filename: conversion-workflows-api-openapi.yml
  format: yaml
  label: Conversion Workflows API
  slug: conversion-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conversion/openapi/conversion-workflows-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Conversion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conversion declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Conversion
provider_slug: conversion
scheme_count: 2
schemes:
- description: API key in X-API-Key header (recommended)
  in: header
  name: X-API-Key
  type: apiKey
- description: API key as query parameter (fallback)
  in: query
  name: api_key
  type: apiKey
slug: conversion-authentication
source_filename: conversion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://docs.conversion.ai/api-reference/authentication.md\nschemes:\n  - type: apiKey\n    name: X-API-Key\n    in: header\n    description: API key in X-API-Key header (recommended)\n  - type: apiKey\n    name: api_key\n    in: query\n    description: API key as query parameter (fallback)"
source_yaml_url: https://artifacts.apis.io/conversion/authentication/conversion-authentication.yml
summary_line: 2 schemes
tags:
- Marketing
- Automation
- AI
- B2B
- SaaS
- Platform
---
