---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Css Authentication
name_suffix: Authentication
oauth_flows: []
overview: CSS (Cascading Style Sheets) declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: CSS (Cascading Style Sheets)
provider_slug: css
scheme_count: 0
schemes: []
slug: css-authentication
source_filename: css-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://jigsaw.w3.org/css-validator/manual.html#requestformat\ndocs: https://jigsaw.w3.org/css-validator/api.html\napi: W3C CSS Validation Service\nsummary: >-\n  The W3C CSS Validation Service is an open, anonymous, unauthenticated web service. It\n  issues no credentials, has no sign-up, no API key, no OAuth and no token of any kind. The\n  User Manual states plainly that it is \"a free, public service for all\" and asks callers to\n  self-throttle instead of authenticating. An agent needs no secret to call it; what it needs\n  is the courtesy rate limit recorded in rate-limits/css-rate-limits.yml.\nmodel: anonymous\nschemes: []\ncredentials_required: false\nsign_up_required: false\ntransport:\n  https: true\n  http_methods: [GET, POST]\n  note: >-\n    POST is used for the file-upload form; the programmatic interface documented in the User\n    Manual is a plain HTTP GET against the base URI with query parameters.\nidentity_signals:\n\
  \  - signal: none\n    note: >-\n      No account, tenant or caller identity exists. Requests are distinguished only by the\n      document being validated, which is echoed back as the uri/TestSubject field.\nself_hosting:\n  note: >-\n    The same servlet can be run privately (java -jar css-validator.jar, or deployed as a war\n    under Tomcat or Jigsaw), in which case the operator supplies whatever authentication their\n    container enforces. See cli/css-cli.yml.\n  source: https://jigsaw.w3.org/css-validator/DOWNLOAD.html\nverification:\n  probed: '2026-09-07'\n  url: https://jigsaw.w3.org/css-validator/validator?text=a%7Bcolor%3Ared%7D&output=json&profile=css3\n  http_status: 200\n  note: >-\n    Called with no credentials of any kind and returned a complete validation result, which\n    confirms the anonymous model rather than inferring it from prose.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/css/refs/heads/main/authentication/css-authentication.yml
summary_line: 0 schemes
tags:
- CSS
- Web Standards
- W3C
- Styling
- Browser
- Specifications
- Validation
- CSSOM
- Houdini
- Front End
---
