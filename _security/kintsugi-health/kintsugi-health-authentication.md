---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kintsugi-health-feedback-api-openapi.yml
  format: yaml
  label: Kintsugi Health Feedback API
  slug: kintsugi-health-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi-health/refs/heads/main/openapi/kintsugi-health-feedback-api-openapi.yml
- filename: kintsugi-health-initiate-api-openapi.yml
  format: yaml
  label: Kintsugi Health Initiate API
  slug: kintsugi-health-initiate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi-health/refs/heads/main/openapi/kintsugi-health-initiate-api-openapi.yml
- filename: kintsugi-health-kintsugi-health-api-api-openapi.yml
  format: yaml
  label: Kintsugi Health Kintsugi Health API
  slug: kintsugi-health-kintsugi-health-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi-health/refs/heads/main/openapi/kintsugi-health-kintsugi-health-api-api-openapi.yml
- filename: kintsugi-health-predict-api-openapi.yml
  format: yaml
  label: Kintsugi Health Predict API
  slug: kintsugi-health-predict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi-health/refs/heads/main/openapi/kintsugi-health-predict-api-openapi.yml
- filename: kintsugi-health-prediction-api-openapi.yml
  format: yaml
  label: Kintsugi Health Prediction API
  slug: kintsugi-health-prediction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kintsugi-health/refs/heads/main/openapi/kintsugi-health-prediction-api-openapi.yml
auth_types: []
description: The KV API uses a unique API key that is provisioned specifically for your organization to authenticate your API requests.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kintsugi Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kintsugi Health declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kintsugi Health
provider_slug: kintsugi-health
scheme_count: 1
schemes:
- evidence: The KV API uses a unique API key that is provisioned specifically for your organization to authenticate your API requests.
  how_to_obtain: Send an email to engineering@kintsugihealth.com with the name of your organization, the email that needs access, and the intended use of Kintsugi Voice. After approval, you will receive an activation token via email, which you submit to generate your API key.
  name: API Key
  type: apiKey
slug: kintsugi-health-authentication
source_filename: kintsugi-health-authentication.yml
source_heading: Authentication Profile
source_url: https://www.kintsugihealth.com/api/get-started
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.kintsugihealth.com/api/get-started\nsources:\n- https://www.kintsugihealth.com/api/get-started\ndescription: The KV API uses a unique API key that is provisioned specifically for your organization to authenticate your API requests.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: The KV API uses a unique API key that is provisioned specifically for your organization to authenticate your API requests.\n  how_to_obtain: Send an email to engineering@kintsugihealth.com with the name of your organization, the email that needs access, and the intended\n    use of Kintsugi Voice. After approval, you will receive an activation token via email, which you submit to generate your API key.\ndocs: https://www.kintsugihealth.com/api/get-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kintsugi-health/refs/heads/main/authentication/kintsugi-health-authentication.yml
summary_line: 1 scheme
tags:
- Health Tech
- Artificial Intelligence
- VoiceAnalytics
- Mental Health
- Digital Health
---
