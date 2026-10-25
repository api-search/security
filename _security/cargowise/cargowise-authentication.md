---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cargowise Authentication
name_suffix: Authentication
oauth_flows: []
overview: CargoWise declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CargoWise
provider_slug: cargowise
scheme_count: 3
schemes:
- description: EDI Client Inbound tab "Authorization Type to OAU (OAuth Authentication)"; a Certificate Signing Request is uploaded and a certificate "issued by WiseTech" is generated, and the integrator receives an "OAuth Authority URL and OAuth Client ID".
  evidence: https://help.logixboard.com/en/articles/15888871-cargowise-eadaptor-next-migration
  name: eAdaptor Next inbound OAuth (OAU)
  type: oauth2
- description: EDI Client Outbound tab "Authorization Type to BAU (Basic Authentication)" with the receiving endpoint, username and password.
  evidence: https://help.logixboard.com/en/articles/15888871-cargowise-eadaptor-next-migration
  name: eAdaptor outbound Basic (BAU)
  scheme: basic
  type: http
- description: Integrators request the inbound eAdapter username, password and URL plus Enterprise ID, Company Code and Server ID.
  evidence: https://docs.bravotran.com/Full-Setup-ec68b67e7ac942a7a3cd3231d9d2ac56
  name: eAdaptor inbound username/password
  scheme: basic
  type: http
slug: cargowise-authentication
source_filename: cargowise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: searched\nsource: https://help.logixboard.com/en/articles/15888871-cargowise-eadaptor-next-migration\ndocs: https://help.logixboard.com/en/articles/15888871-cargowise-eadaptor-next-migration\nnote: >-\n  WiseTech publishes no public authentication reference; the eAdaptor Developers Guide is customer-gated.\n  The schemes below are as described by third-party integrators configuring a CargoWise EDI Client, not by\n  WiseTech itself.\nschemes:\n- name: eAdaptor Next inbound OAuth (OAU)\n  type: oauth2\n  description: >-\n    EDI Client Inbound tab \"Authorization Type to OAU (OAuth Authentication)\"; a Certificate Signing Request is\n    uploaded and a certificate \"issued by WiseTech\" is generated, and the integrator receives an \"OAuth Authority\n    URL and OAuth Client ID\".\n  evidence: https://help.logixboard.com/en/articles/15888871-cargowise-eadaptor-next-migration\n- name: eAdaptor outbound Basic (BAU)\n  type: http\n  scheme: basic\n\
  \  description: EDI Client Outbound tab \"Authorization Type to BAU (Basic Authentication)\" with the receiving endpoint, username and password.\n  evidence: https://help.logixboard.com/en/articles/15888871-cargowise-eadaptor-next-migration\n- name: eAdaptor inbound username/password\n  type: http\n  scheme: basic\n  description: Integrators request the inbound eAdapter username, password and URL plus Enterprise ID, Company Code and Server ID.\n  evidence: https://docs.bravotran.com/Full-Setup-ec68b67e7ac942a7a3cd3231d9d2ac56\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargowise/refs/heads/main/authentication/cargowise-authentication.yml
summary_line: 3 schemes
tags:
- Logistics
- Freight Forwarding
- Supply Chain
- Customs
- Shipping
- eAdaptor
- Universal XML
- EDI
- WiseTech Global
---
