---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: The Mobility House Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Mobility House declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: The Mobility House
provider_slug: the-mobility-house
scheme_count: 4
schemes:
- api: the-mobility-house-chargepilot-vdv-463
  credential_issuance: Manual. The customer requests a ChargePilot site be enabled for VDV 463; The Mobility House configures the site, generates customer-specific credentials, and delivers them together with a recommended TMH certificate. There is no self-service key issuance.
  description: Customers identify themselves during the VDV 463 WebSocket TLS handshake using HTTP Basic Authentication with a username and password issued by The Mobility House when the site is configured for VDV 463.
  id: vdv463-http-basic
  location: WebSocket upgrade request (Authorization header, credentials Base64-encoded)
  rotation: not documented
  scheme: basic
  scopes: none documented
  transport_security: TLS mandatory — VDV 463 defines WebSocket Secure as the transport. The Mobility House additionally recommends pinning the certificate it supplies to prevent unauthorized access.
  type: http
- api: the-mobility-house-chargepilot-charging-data-push-api
  credential_issuance: Agreed during Push-API onboarding with the customer success manager.
  description: 'ChargePilot presents an Azure API Management subscription key to the customer-operated receiving endpoint when POSTing charging session data. The direction is inverted relative to a normal API key: the provider authenticates itself to the consumer.'
  id: push-api-subscription-key
  in: header
  name: Ocp-Apim-Subscription-Key
  rotation: not documented
  scopes: none documented
  type: apiKey
- api: chargepilot-modbus-interface
  description: 'The ChargePilot / TMH Controller Modbus TCP/IP server exposes no authentication. Access control is network-level only: the interface is deactivated by default, must be enabled by a customer success manager, is reachable on the local site network at a configurable IP with slave ID 1, and can be restricted to read-only (input registers) or read/write (input plus holding registers).'
  id: modbus-tcp-no-auth
  rotation: n/a
  scopes: n/a
  type: none
- api: chargepilot-ocpp
  description: Charging stations connect into ChargePilot over OCPP. OCPP 1.6-J and 2.0.1 station authentication is defined by the OCPP standard rather than by a Mobility House-specific scheme; The Mobility House does not publish its per-station credential policy.
  id: ocpp-station-auth
  note: Recorded for completeness of the auth surface; not independently verified against a Mobility House document.
  scheme: basic
  type: http
slug: the-mobility-house-authentication
source_filename: the-mobility-house-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: searched\nsource: 'https://vdv-docs.tmh.energy/initial-connection/initial-connection/ and\n  https://tmh-help.freshdesk.com/en/support/solutions/articles/203000046009-chargepilot-charging-data-push-api\n  and https://tmh-help.freshdesk.com/en/support/solutions/articles/203000046016-chargepilot-modbus-interface,\n  fetched 2026-08-30. Derived nothing from OpenAPI: The Mobility House publishes no OpenAPI or Swagger\n  document, so there are no securitySchemes to read.'\ndocs: https://vdv-docs.tmh.energy/initial-connection/initial-connection/\nname: The Mobility House authentication profile\nopenapi_security_schemes: 0\nschemes:\n- id: vdv463-http-basic\n  api: the-mobility-house-chargepilot-vdv-463\n  type: http\n  scheme: basic\n  location: 'WebSocket upgrade request (Authorization header, credentials Base64-encoded)'\n  description: 'Customers identify themselves during the VDV 463 WebSocket TLS handshake using HTTP\n    Basic Authentication\
  \ with a username and password issued by The Mobility House when the site is\n    configured for VDV 463.'\n  credential_issuance: 'Manual. The customer requests a ChargePilot site be enabled for VDV 463; The\n    Mobility House configures the site, generates customer-specific credentials, and delivers them\n    together with a recommended TMH certificate. There is no self-service key issuance.'\n  transport_security: 'TLS mandatory — VDV 463 defines WebSocket Secure as the transport. The Mobility\n    House additionally recommends pinning the certificate it supplies to prevent unauthorized access.'\n  rotation: not documented\n  scopes: none documented\n- id: push-api-subscription-key\n  api: the-mobility-house-chargepilot-charging-data-push-api\n  type: apiKey\n  in: header\n  name: Ocp-Apim-Subscription-Key\n  description: 'ChargePilot presents an Azure API Management subscription key to the customer-operated\n    receiving endpoint when POSTing charging session data. The direction\
  \ is inverted relative to a\n    normal API key: the provider authenticates itself to the consumer.'\n  credential_issuance: 'Agreed during Push-API onboarding with the customer success manager.'\n  rotation: not documented\n  scopes: none documented\n- id: modbus-tcp-no-auth\n  api: chargepilot-modbus-interface\n  type: none\n  description: 'The ChargePilot / TMH Controller Modbus TCP/IP server exposes no authentication. Access\n    control is network-level only: the interface is deactivated by default, must be enabled by a\n    customer success manager, is reachable on the local site network at a configurable IP with slave\n    ID 1, and can be restricted to read-only (input registers) or read/write (input plus holding\n    registers).'\n  rotation: n/a\n  scopes: n/a\n- id: ocpp-station-auth\n  api: chargepilot-ocpp\n  type: http\n  scheme: basic\n  description: 'Charging stations connect into ChargePilot over OCPP. OCPP 1.6-J and 2.0.1 station\n    authentication is defined by the\
  \ OCPP standard rather than by a Mobility House-specific scheme;\n    The Mobility House does not publish its per-station credential policy.'\n  note: 'Recorded for completeness of the auth surface; not independently verified against a Mobility\n    House document.'\noauth2: false\nopenid_connect: false\nmutual_tls: 'partial — a TMH-issued certificate is recommended (not documented as required) on the\n  VDV 463 connection.'\nself_service_signup: false\nsignup_path: 'Sales / customer success. https://www.mobilityhouse.com/int_en/contact'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-mobility-house/refs/heads/main/authentication/the-mobility-house-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Energy
- Electric Vehicles
- EV Charging
- Smart Charging
- Energy Management
- Vehicle-to-Grid
- Load Management
- Fleet
- OCPP
- VDV 463
- Modbus
- Germany
---
