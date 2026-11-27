---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for EduBase API as published on the documentation pages.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: EduBase Authentication
name_suffix: Authentication
oauth_flows: []
overview: EduBase declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: EduBase
provider_slug: edubase-net
scheme_count: 3
schemes:
- evidence: 'All endpoints require a valid application ID and secret . They should be passed as arguments: app : this is the application identification string secret : the application secret string'
  how_to_obtain: Provided when registering an application in the EduBase developer portal.
  location: query
  name: Application ID and secret as arguments
  type: apiKey
- evidence: Alternatively, you can use the Authorization header with the value Bearer {app}:{secret}
  header: Authorization
  how_to_obtain: Application ID and secret are obtained during application registration.
  location: header
  name: Authorization header Bearer {app}:{secret}
  type: http-bearer
- evidence: or dedicated EduBase-API-App and EduBase-API-Secret headers.
  header: EduBase-API-App, EduBase-API-Secret
  how_to_obtain: Application ID and secret are obtained during application registration.
  location: header
  name: Dedicated EduBase-API-App and EduBase-API-Secret headers
  type: apiKey
slug: edubase-net-authentication
source_filename: edubase-net-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.edubase.net/api/authentication/
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.edubase.net/api/authentication/\nsources:\n- https://developer.edubase.net/api/authentication/\n- https://help.edubase.net/getting-started/1-registering-to-edubase/\n- https://help.edubase.net/getting-started/2-customizing-the-dashboard/\n- https://help.edubase.net/getting-started/3-creating-a-classroom/\ndescription: Authentication methods for EduBase API as published on the documentation pages.\nschemes:\n- type: apiKey\n  name: Application ID and secret as arguments\n  evidence: 'All endpoints require a valid application ID and secret . They should be passed as arguments: app : this is the application identification\n    string secret : the application secret string'\n  location: query\n  how_to_obtain: Provided when registering an application in the EduBase developer portal.\n- type: http-bearer\n  name: Authorization header Bearer {app}:{secret}\n  evidence:\
  \ Alternatively, you can use the Authorization header with the value Bearer {app}:{secret}\n  location: header\n  header: Authorization\n  how_to_obtain: Application ID and secret are obtained during application registration.\n- type: apiKey\n  name: Dedicated EduBase-API-App and EduBase-API-Secret headers\n  evidence: or dedicated EduBase-API-App and EduBase-API-Secret headers.\n  location: header\n  header: EduBase-API-App, EduBase-API-Secret\n  how_to_obtain: Application ID and secret are obtained during application registration.\nnote: No OAuth2 flows, JWT, HMAC, MTLS, or other authentication schemes are documented.\ndocs: https://developer.edubase.net/api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/edubase-net/authentication/edubase-net-authentication.yml
summary_line: 3 schemes
tags:
- Education
- LMS
- E-Learning
- Company
---
