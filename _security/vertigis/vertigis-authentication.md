---
api_key_in: []
auth_types:
- oauth2
- token
description: ''
kind: authentication
layout: security
method: searched
name: Vertigis Authentication
name_suffix: Authentication
oauth_flows: []
overview: VertiGIS secures its APIs with oauth2 and token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VertiGIS
provider_slug: vertigis
scheme_count: 2
schemes:
- description: ArcGIS access token passed to the Reporting/Printing REST service (or supplied to the JavaScript/Python reporting client) to authorize a job. Acquired from the ArcGIS portal.
  in: query
  name: ArcGISToken
  parameter: token
  type: apiKey
- authorization_provider: ArcGIS Online / ArcGIS Enterprise
  description: OAuth 2.0 named-user or app login handled by Esri ArcGIS Identity; VertiGIS Studio applications and SDKs consume the resulting portal token.
  flow: authorizationCode
  name: ArcGISOAuth2
  type: oauth2
slug: vertigis-authentication
source_filename: vertigis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.vertigisstudio.com/docs/reporting/sdk-overview/\ndocs: https://developers.vertigisstudio.com/docs/web/sdk-services-reference/\nsummary:\n  types: [oauth2, token]\n  identity_provider: Esri ArcGIS Identity (ArcGIS Online / ArcGIS Enterprise Portal)\n  notes: >-\n    VertiGIS Studio does not issue its own credentials. Access to the Reporting REST\n    API, Web, Mobile, and Workflow services is authorized with an ArcGIS access token\n    obtained from the user's ArcGIS Online or ArcGIS Enterprise portal via OAuth 2.0,\n    then passed to the VertiGIS service. Anonymous access is possible for\n    unsecured maps and public reporting templates.\nschemes:\n- name: ArcGISToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: >-\n    ArcGIS access token passed to the Reporting/Printing REST service (or supplied to\n    the JavaScript/Python reporting client) to authorize a job. Acquired from the\n\
  \    ArcGIS portal.\n- name: ArcGISOAuth2\n  type: oauth2\n  flow: authorizationCode\n  authorization_provider: ArcGIS Online / ArcGIS Enterprise\n  description: >-\n    OAuth 2.0 named-user or app login handled by Esri ArcGIS Identity; VertiGIS Studio\n    applications and SDKs consume the resulting portal token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vertigis/refs/heads/main/authentication/vertigis-authentication.yml
summary_line: oauth2/token · 2 schemes
tags:
- Company
- GIS
- Geospatial
- Mapping
- ArcGIS
- Esri
- Location Intelligence
- Reporting
- SDK
- Developer Tools
- Workflow Automation
- Utilities
---
