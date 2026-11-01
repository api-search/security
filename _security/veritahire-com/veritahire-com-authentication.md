---
anonymous_access: false
api_key_in: []
api_specs:
- filename: veritahire-com-account-api-openapi.yml
  format: yaml
  label: veritahire-com Account API
  slug: veritahire-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veritahire-com/openapi/veritahire-com-account-api-openapi.yml
- filename: veritahire-com-employer-profile-api-openapi.yml
  format: yaml
  label: veritahire-com Employer profile API
  slug: veritahire-com-employer-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veritahire-com/openapi/veritahire-com-employer-profile-api-openapi.yml
- filename: veritahire-com-free-no-key-api-openapi.yml
  format: yaml
  label: veritahire-com Free, no key API
  slug: veritahire-com-free-no-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veritahire-com/openapi/veritahire-com-free-no-key-api-openapi.yml
- filename: veritahire-com-hiring-market-php-api-openapi.yml
  format: yaml
  label: veritahire-com Hiring Market.php API
  slug: veritahire-com-hiring-market-php-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veritahire-com/openapi/veritahire-com-hiring-market-php-api-openapi.yml
- filename: veritahire-com-hiring-velocity-api-openapi.yml
  format: yaml
  label: veritahire-com Hiring velocity API
  slug: veritahire-com-hiring-velocity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veritahire-com/openapi/veritahire-com-hiring-velocity-api-openapi.yml
- filename: veritahire-com-postings-api-openapi.yml
  format: yaml
  label: veritahire-com Postings API
  slug: veritahire-com-postings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/veritahire-com/openapi/veritahire-com-postings-api-openapi.yml
auth_types: []
description: Authentication for VeritaHire Jobs API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Veritahire Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: veritahire-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: veritahire-com
provider_slug: veritahire-com
scheme_count: 1
schemes:
- evidence: 'From a script: GET https://veritahire.com/api/v1/balance.php with your key in the X-API-Key header.'
  header: X-API-Key
  how_to_obtain: Get a free key first →
  location: header
  name: API Key
  type: apiKey
slug: veritahire-com-authentication
source_filename: veritahire-com-authentication.yml
source_heading: Authentication Profile
source_url: https://veritahire.com/verified-jobs-feed/
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://veritahire.com/verified-jobs-feed/\nsources:\n- https://veritahire.com/verified-jobs-feed/\ndescription: Authentication for VeritaHire Jobs API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'From a script: GET https://veritahire.com/api/v1/balance.php with your key in the X-API-Key header.'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Get a free key first →\ndocs: https://veritahire.com/verified-jobs-feed/\n"
source_yaml_url: https://artifacts.apis.io/veritahire-com/authentication/veritahire-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Jobs
- Hiring
- API
- Data
---
