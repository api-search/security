---
api_key_in: []
api_specs:
- filename: adobe-captivate-learning-manager-webhooks-asyncapi.yml
  format: yaml
  label: Adobe Learning Manager Webhooks API
  slug: adobe-learning-manager-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/asyncapi/adobe-captivate-learning-manager-webhooks-asyncapi.yml
- filename: adobe-captivate-account-api-openapi.yml
  format: yaml
  label: Adobe Captivate Account API
  slug: adobe-captivate-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-account-api-openapi.yml
- filename: adobe-captivate-badges-api-openapi.yml
  format: yaml
  label: Adobe Captivate Badges API
  slug: adobe-captivate-badges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-badges-api-openapi.yml
- filename: adobe-captivate-catalogs-api-openapi.yml
  format: yaml
  label: Adobe Captivate Catalogs API
  slug: adobe-captivate-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-catalogs-api-openapi.yml
- filename: adobe-captivate-certifications-api-openapi.yml
  format: yaml
  label: Adobe Captivate Certifications API
  slug: adobe-captivate-certifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-certifications-api-openapi.yml
- filename: adobe-captivate-enrollments-api-openapi.yml
  format: yaml
  label: Adobe Captivate Enrollments API
  slug: adobe-captivate-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-enrollments-api-openapi.yml
- filename: adobe-captivate-gamification-api-openapi.yml
  format: yaml
  label: Adobe Captivate Gamification API
  slug: adobe-captivate-gamification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-gamification-api-openapi.yml
- filename: adobe-captivate-jobs-api-openapi.yml
  format: yaml
  label: Adobe Captivate Jobs API
  slug: adobe-captivate-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-jobs-api-openapi.yml
- filename: adobe-captivate-learning-objects-api-openapi.yml
  format: yaml
  label: Adobe Captivate Learning Objects API
  slug: adobe-captivate-learning-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-learning-objects-api-openapi.yml
- filename: adobe-captivate-notifications-api-openapi.yml
  format: yaml
  label: Adobe Captivate Notifications API
  slug: adobe-captivate-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-notifications-api-openapi.yml
- filename: adobe-captivate-skills-api-openapi.yml
  format: yaml
  label: Adobe Captivate Skills API
  slug: adobe-captivate-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-skills-api-openapi.yml
- filename: adobe-captivate-user-groups-api-openapi.yml
  format: yaml
  label: Adobe Captivate User Groups API
  slug: adobe-captivate-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-user-groups-api-openapi.yml
- filename: adobe-captivate-users-api-openapi.yml
  format: yaml
  label: Adobe Captivate Users API
  slug: adobe-captivate-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/openapi/adobe-captivate-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Captivate Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Adobe Captivate secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Adobe Captivate
provider_slug: adobe-captivate
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication via Adobe IMS. Supports authorization code flow for user-context access and client credentials flow for application-level access.
  flows:
  - authorizationUrl: https://learningmanager.adobe.com/oauth/o/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://learningmanager.adobe.com/oauth/token
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://learningmanager.adobe.com/oauth/token
  name: oauth2
  sources:
  - openapi/adobe-captivate-prime-api-openapi.yml
  type: oauth2
slug: adobe-captivate-authentication
source_filename: adobe-captivate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-captivate-prime-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://learningmanager.adobe.com/oauth/o/authorize\n    tokenUrl: https://learningmanager.adobe.com/oauth/token\n    scopes: 4\n  - flow: clientCredentials\n    tokenUrl: https://learningmanager.adobe.com/oauth/token\n    scopes: 3\n  description: OAuth 2.0 authentication via Adobe IMS. Supports authorization code flow for\n    user-context access and client credentials flow for application-level access.\n  sources:\n  - openapi/adobe-captivate-prime-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/authentication/adobe-captivate-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
---
