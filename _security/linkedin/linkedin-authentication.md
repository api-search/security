---
api_key_in: []
api_specs:
- filename: linkedin-marketing-audience-insights.yml
  format: yaml
  label: LinkedIn Marketing API
  slug: linkedin-marketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/openapi/linkedin-marketing-audience-insights.yml
- filename: linkedin-learning-activity-reports.yml
  format: yaml
  label: LinkedIn Learning Solutions
  slug: linkedin-learning-solutions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/openapi/linkedin-learning-activity-reports.yml
- filename: linkedin-talent-job-posting.yml
  format: yaml
  label: LinkedIn Talent Solutions
  slug: linkedin-talent-solutions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/openapi/linkedin-talent-job-posting.yml
- filename: linkedin-compliance-events.yml
  format: yaml
  label: LinkedIn Compliance Solutions
  slug: linkedin-compliance-solutions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/openapi/linkedin-compliance-events.yml
- filename: linkedin-sales-navigator.yml
  format: yaml
  label: LinkedIn Sales Navigator API
  slug: linkedin-sales-navigator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/openapi/linkedin-sales-navigator.yml
- filename: linkedin-regulations-data-portability.yml
  format: yaml
  label: LinkedIn Regulatory API
  slug: linkedin-regulatory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/openapi/linkedin-regulations-data-portability.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Linkedin Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: LinkedIn secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: LinkedIn
provider_slug: linkedin
scheme_count: 4
schemes:
- flows:
  - authorizationUrl: https://www.linkedin.com/oauth/v2/authorization
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2Auth
  sources:
  - openapi/linkedin-compliance-events.yml
  - openapi/linkedin-learning-activity-reports.yml
  - openapi/linkedin-marketing-audience-insights.yml
  - openapi/linkedin-marketing-audience.yml
  - openapi/linkedin-marketing-campaigns.yml
  - openapi/linkedin-talent-recruiter-system-connect.yml
  type: oauth2
- name: oauth2Auth
  scheme: oauth2
  sources:
  - openapi/linkedin-marketing-community.yml
  - openapi/linkedin-marketing-content.yml
  - openapi/linkedin-marketing-conversions.yml
  - openapi/linkedin-marketing-leads.yml
  - openapi/linkedin-marketing-reporting-roi.yml
  type: http
- description: OAuth 2.0 Bearer Token for API access
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/linkedin-regulations-data-portability.yml
  - openapi/linkedin-regulatory-ads-transparency.yml
  - openapi/linkedin-sales-navigator.yml
  - openapi/linkedin-talent-job-posting.yml
  - openapi/linkedin-talent-recruiter-system-connect.yml
  type: http
- description: OAuth 2.0 authentication
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken
  name: OAuth2Auth
  sources:
  - openapi/linkedin-talent-job-posting.yml
  - openapi/linkedin-talent-learning-parent-application.yml
  type: oauth2
slug: linkedin-authentication
source_filename: linkedin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/linkedin-compliance-events.yml, openapi/linkedin-learning-activity-reports.yml,\n  openapi/linkedin-marketing-audience-insights.yml, openapi/linkedin-marketing-audience.yml,\n  openapi/linkedin-marketing-campaigns.yml, openapi/linkedin-marketing-community.yml, openapi/linkedin-marketing-content.yml,\n  openapi/linkedin-marketing-conversions.yml, openapi/linkedin-marketing-leads.yml, openapi/linkedin-marketing-reporting-roi.yml,\n  openapi/linkedin-regulations-data-portability.yml, openapi/linkedin-regulatory-ads-transparency.yml\n  ...\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2Auth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.linkedin.com/oauth/v2/authorization\n    tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n    scopes: 1\n  sources:\n  - openapi/linkedin-compliance-events.yml\n\
  \  - openapi/linkedin-learning-activity-reports.yml\n  - openapi/linkedin-marketing-audience-insights.yml\n  - openapi/linkedin-marketing-audience.yml\n  - openapi/linkedin-marketing-campaigns.yml\n  - openapi/linkedin-talent-recruiter-system-connect.yml\n- name: oauth2Auth\n  type: http\n  scheme: oauth2\n  sources:\n  - openapi/linkedin-marketing-community.yml\n  - openapi/linkedin-marketing-content.yml\n  - openapi/linkedin-marketing-conversions.yml\n  - openapi/linkedin-marketing-leads.yml\n  - openapi/linkedin-marketing-reporting-roi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer Token for API access\n  sources:\n  - openapi/linkedin-regulations-data-portability.yml\n  - openapi/linkedin-regulatory-ads-transparency.yml\n  - openapi/linkedin-sales-navigator.yml\n  - openapi/linkedin-talent-job-posting.yml\n  - openapi/linkedin-talent-recruiter-system-connect.yml\n- name: OAuth2Auth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n  \
  \  tokenUrl: https://www.linkedin.com/oauth/v2/accessToken\n    scopes: 1\n  description: OAuth 2.0 authentication\n  sources:\n  - openapi/linkedin-talent-job-posting.yml\n  - openapi/linkedin-talent-learning-parent-application.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/authentication/linkedin-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
- Fortune 1000
---
