---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coupure-Elec.fr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coupure-Elec.fr declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Coupure-Elec.fr
provider_slug: coupure-elec-fr
scheme_count: 1
schemes:
- applies_to: https://www.coupure-elec.fr/api/mcp
  header: Authorization
  in: header
  key_prefix: ce_live_
  name: partnerBearerKey
  provisioning: Request form on the MCP page ("Demander une clé MCP"); the page says it replies within 48 business hours.
  quote: 'Authentification par en-tête Authorization: Bearer ce_live_…'
  scheme: bearer
  type: http
slug: coupure-elec-fr-authentication
source_filename: coupure-elec-fr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.coupure-elec.fr/mcp\ndocs: https://www.coupure-elec.fr/mcp\nsummary: The remote MCP server (Streamable HTTP, https://www.coupure-elec.fr/api/mcp) authenticates with a partner bearer key (prefix ce_live_) in the Authorization header. Keys are issued by hand after a request form is approved (\"Sans compte Une simple clé partenaire, remise après validation de votre demande\"). No OAuth flow is documented. The endpoint answered 401 to an unauthenticated probe (pre-flight, 2026-11-04).\nschemes:\n- name: partnerBearerKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  key_prefix: ce_live_\n  quote: \"Authentification par en-tête Authorization: Bearer ce_live_…\"\n  applies_to: https://www.coupure-elec.fr/api/mcp\n  provisioning: Request form on the MCP page (\"Demander une clé MCP\"); the page says it replies within 48 business hours.\n"
source_yaml_url: https://artifacts.apis.io/coupure-elec-fr/authentication/coupure-elec-fr-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Electricity
- Power Outages
- Energy
- France
- MCP
- Crowdsourcing
- Open Data
---
