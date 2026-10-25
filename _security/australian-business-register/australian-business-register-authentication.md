---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Australian Business Register Authentication
name_suffix: Authentication
oauth_flows: []
overview: Australian Business Register declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Australian Business Register
provider_slug: australian-business-register
scheme_count: 1
schemes:
- description: 'Registered users get an authentication GUID by email after they accept the web services agreement. The docs say: ''We will process your application and e-mail you an authentication GUID (Globally Unique Identifier) which is required to access the ABN Lookup web services.'' The GUID is sent as a request element (authenticationGuid / authenticationGUID) on every SOAP or HTTP GET/POST method, and as the guid parameter on the JSONP services.'
  errors:
  - The GUID entered is not recognised as a Registered Party
  - The party identified by this GUID has not been registered for the requested service
  in: query
  name: authenticationGuid
  obtain: https://abr.business.gov.au/Documentation/WebServiceRegistration
  parameter: authenticationGuid
  type: apiKey
slug: australian-business-register-authentication
source_filename: australian-business-register-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: searched\nsource: https://abr.business.gov.au/Documentation/WebServiceRegistration\ndocs: https://abr.business.gov.au/Documentation/WebServiceMethods\nschemes:\n- name: authenticationGuid\n  type: apiKey\n  in: query\n  parameter: authenticationGuid\n  description: \"Registered users get an authentication GUID by email after they accept the web services agreement. The docs say: 'We will process your application and e-mail you an authentication GUID (Globally Unique Identifier) which is required to access the ABN Lookup web services.' The GUID is sent as a request element (authenticationGuid / authenticationGUID) on every SOAP or HTTP GET/POST method, and as the guid parameter on the JSONP services.\"\n  obtain: https://abr.business.gov.au/Documentation/WebServiceRegistration\n  errors:\n  - The GUID entered is not recognised as a Registered Party\n  - The party identified by this GUID has not been registered for the requested service\nnote:\
  \ There is no OAuth, so no scopes artifact. The credential is a long-lived shared GUID, not a signed token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-business-register/refs/heads/main/authentication/australian-business-register-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Government
- Australia
- Business Registry
- ABN
- Tax
- Public Sector
- Open Data
---
