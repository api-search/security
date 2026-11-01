---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: deepl-voice-api-openapi.yml
  format: yaml
  label: DeepL Voice API
  slug: deepl-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-voice-api-openapi.yml
- filename: deepl-adminapi-api-openapi.yml
  format: yaml
  label: DeepL Admin API
  slug: deepl-adminapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-adminapi-api-openapi.yml
- filename: deepl-correcttext-api-openapi.yml
  format: yaml
  label: DeepL Correct Text API
  slug: deepl-correcttext-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-correcttext-api-openapi.yml
- filename: deepl-manageglossaries-api-openapi.yml
  format: yaml
  label: DeepL Manage Glossaries API
  slug: deepl-manageglossaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-manageglossaries-api-openapi.yml
- filename: deepl-managemultilingualglossaries-api-openapi.yml
  format: yaml
  label: DeepL Manage Multilingual Glossaries API
  slug: deepl-managemultilingualglossaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-managemultilingualglossaries-api-openapi.yml
- filename: deepl-managespokenterms-api-openapi.yml
  format: yaml
  label: DeepL Manage Spoken Terms API
  slug: deepl-managespokenterms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-managespokenterms-api-openapi.yml
- filename: deepl-metainformation-api-openapi.yml
  format: yaml
  label: DeepL Meta Information API
  slug: deepl-metainformation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-metainformation-api-openapi.yml
- filename: deepl-qualityevaluation-api-openapi.yml
  format: yaml
  label: DeepL Quality Evaluation API
  slug: deepl-qualityevaluation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-qualityevaluation-api-openapi.yml
- filename: deepl-rephrasetext-api-openapi.yml
  format: yaml
  label: DeepL Rephrase Text API
  slug: deepl-rephrasetext-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-rephrasetext-api-openapi.yml
- filename: deepl-style-rules-api-openapi.yml
  format: yaml
  label: DeepL Style Rules API
  slug: deepl-style-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-style-rules-api-openapi.yml
- filename: deepl-translatedocuments-api-openapi.yml
  format: yaml
  label: DeepL Translate Documents API
  slug: deepl-translatedocuments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-translatedocuments-api-openapi.yml
- filename: deepl-translatetext-api-openapi.yml
  format: yaml
  label: DeepL Translate Text API
  slug: deepl-translatetext-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-translatetext-api-openapi.yml
- filename: deepl-translationmemories-api-openapi.yml
  format: yaml
  label: DeepL Translation Memories API
  slug: deepl-translationmemories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-translationmemories-api-openapi.yml
- filename: deepl-voiceapi-api-openapi.yml
  format: yaml
  label: DeepL Voice API
  slug: deepl-voiceapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-voiceapi-api-openapi.yml
- filename: deepl-voicetranslatejob-api-openapi.yml
  format: yaml
  label: DeepL Voice Translate Job API
  slug: deepl-voicetranslatejob-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepl/openapi/deepl-voicetranslatejob-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Deepl Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeepL secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DeepL
provider_slug: deepl
scheme_count: 1
schemes:
- description: DeepL-Auth-Key <key>
  in: header
  name: authKey
  parameter: Authorization
  sources:
  - openapi/deepl-translation-api-openapi.yml
  - openapi/deepl-voice-api-openapi.yml
  type: apiKey
slug: deepl-authentication
source_filename: deepl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deepl-translation-api-openapi.yml, openapi/deepl-voice-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: authKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: DeepL-Auth-Key <key>\n  sources:\n  - openapi/deepl-translation-api-openapi.yml\n  - openapi/deepl-voice-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/deepl/authentication/deepl-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Deep Learning
- Glossary
- Localization
- Machine Learning
- Machine Translation
- Translation
- Real-Time
---
