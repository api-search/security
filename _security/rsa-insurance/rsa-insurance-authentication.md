---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Rsa Insurance Authentication
name_suffix: Authentication
oauth_flows: []
overview: RSA Insurance declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: RSA Insurance
provider_slug: rsa-insurance
scheme_count: 4
schemes:
- audience: registered insurance intermediaries
  covers:
  - Claims Online
  - Documents Online
  - MID Updates
  current_host: https://www.connect.intactinsurance.co.uk/
  mechanism: User ID + password (HTML form)
  name: rsa-connect-portal-login
  provisioning:
    contact: Intermediated.ebusiness@intactinsurance.co.uk
    method: manual, by email
    quote: '"Welcome to the Connect Intermediary Website ... Our online services such as Claims Online, Documents Online and MID Updates are available in this password protected area. If you are an insurance intermediary and require access please email your request to Intermediated.ebusiness@intactinsurance.co.uk, including your Name, contact details, Agency number."'
    required:
    - name
    - contact details
    - agency number
  surface: https://www.rsaconnect.rsagroup.co.uk/portal/UKHome.aspx
  type: portal-login
- audience: brokers only
  covers:
  - intermediated personal home
  - commercial trading
  mechanism: User ID + password (ASP.NET logon workflow)
  name: rsa-online-trading-login
  surface: https://www.rsaonline.rsagroup.com/AWE/Container.aspx?CurrentWorkflow=Logon&CurrentStep=Login
  type: portal-login
- audience: registered intermediaries
  covers:
  - Motor Insurance Database vehicle uploads and changes
  mechanism: User ID + password
  name: mid2-portal-login
  surface: https://www.services1.rsagroup.co.uk/webappserver/midphase2public/
  type: portal-login
- covers:
  - commercial property first notification of loss
  mechanism: none — unauthenticated public HTML form
  name: commercial-property-efnol
  surface: https://commercial-property-claims.rsabroker.com/rsa_commercial_property/claim/request/
  type: anonymous-web-form
slug: rsa-insurance-authentication
source_filename: rsa-insurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://www.rsainsurance.co.uk/brokers-and-partners/tools-resources/\ndocs: https://www.rsaconnect.rsagroup.co.uk/portal/UKHome.aspx\nsummary:\n  types: []\n  api_authentication: none\n  api_key_in: []\n  oauth2_flows: []\n  human_provisioned: true\n  note: >-\n    RSA Insurance exposes no API and therefore no API authentication. Every\n    scheme below is a human web-portal login, documented on RSA's public broker\n    tools page. There are no API keys, no OAuth 2.0, no OpenID Connect, no mTLS\n    and no published SAML metadata. This artifact records the access model the\n    provider actually publishes so an integrator knows the real onboarding\n    path — email a human — rather than hunting for credentials that do not exist.\nschemes:\n- name: rsa-connect-portal-login\n  type: portal-login\n  mechanism: User ID + password (HTML form)\n  surface: https://www.rsaconnect.rsagroup.co.uk/portal/UKHome.aspx\n  current_host: https://www.connect.intactinsurance.co.uk/\n\
  \  audience: registered insurance intermediaries\n  provisioning:\n    method: manual, by email\n    contact: Intermediated.ebusiness@intactinsurance.co.uk\n    required: [name, contact details, agency number]\n    quote: >-\n      \"Welcome to the Connect Intermediary Website ... Our online services such\n      as Claims Online, Documents Online and MID Updates are available in this\n      password protected area. If you are an insurance intermediary and require\n      access please email your request to\n      Intermediated.ebusiness@intactinsurance.co.uk, including your Name,\n      contact details, Agency number.\"\n  covers: [Claims Online, Documents Online, MID Updates]\n- name: rsa-online-trading-login\n  type: portal-login\n  mechanism: User ID + password (ASP.NET logon workflow)\n  surface: https://www.rsaonline.rsagroup.com/AWE/Container.aspx?CurrentWorkflow=Logon&CurrentStep=Login\n  audience: brokers only\n  covers: [intermediated personal home, commercial trading]\n- name:\
  \ mid2-portal-login\n  type: portal-login\n  mechanism: User ID + password\n  surface: https://www.services1.rsagroup.co.uk/webappserver/midphase2public/\n  audience: registered intermediaries\n  covers: [Motor Insurance Database vehicle uploads and changes]\n- name: commercial-property-efnol\n  type: anonymous-web-form\n  mechanism: none — unauthenticated public HTML form\n  surface: https://commercial-property-claims.rsabroker.com/rsa_commercial_property/claim/request/\n  covers: [commercial property first notification of loss]\nnegative_findings:\n- probe: /.well-known/openid-configuration\n  hosts: [www.rsainsurance.co.uk, www.intactinsurance.co.uk, www.rsaonline.rsagroup.com]\n  status: 404\n- probe: /.well-known/oauth-authorization-server\n  hosts: [www.rsainsurance.co.uk, www.intactinsurance.co.uk, www.rsaonline.rsagroup.com]\n  status: 404\n- probe: /.well-known/openid-configuration\n  hosts: [www.connect.intactinsurance.co.uk, www.rsaconnect.rsagroup.co.uk]\n  status: 200\n  note:\
  \ >-\n    Not OIDC metadata. The ASP.NET front controller rewrites every unknown path\n    to /ErrorPage.aspx with the plain-text body \"Security Error!.. Invalid URL\n    or Invalid data\".\n- probe: SAML metadata\n  result: none published\n- probe: machine-to-machine credentials\n  result: >-\n    None documented. System-to-system trading with RSA runs through broker\n    software houses (Acturis, Applied, Open GI, SSP, Bravo Digital Trader) and\n    the Polaris imarket hub, whose credentials are issued by those parties, not\n    by RSA.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rsa-insurance/refs/heads/main/authentication/rsa-insurance-authentication.yml
summary_line: 4 schemes
tags:
- Insurance
- United Kingdom
- Property and Casualty
- Commercial Lines
- Carrier
- Brokers
- Claims
- Underwriting
- Partner Gated
---
