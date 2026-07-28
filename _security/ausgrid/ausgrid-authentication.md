---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Ausgrid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ausgrid declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Ausgrid
provider_slug: ausgrid
scheme_count: 0
schemes: []
slug: ausgrid-authentication
source_filename: ausgrid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: |\n  Live probes of every Ausgrid-operated host plus the ArcGIS REST endpoints that\n  carry Ausgrid-owned network data; Ausgrid's own meter-data access page.\ndocs: https://www.ausgrid.com.au/your-energy-use/your-meter-and-supply/access-your-meter-data\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  finding: |\n    Ausgrid operates no authenticated API, so there is no security scheme to derive.\n    There is no API key, no OAuth 2.0, no OpenID Connect, no mutual TLS and no bearer\n    token on any published surface. Every machine-readable surface associated with\n    Ausgrid is ANONYMOUS, and the one surface that is genuinely restricted — a\n    customer's own interval meter data — is gated by IDENTITY VERIFICATION on a web\n    form, not by a credential.\nschemes: []\nsurfaces:\n- name: Zone substation interval demand bulk downloads\n  url: https://www.ausgrid.com.au/about-us/about-ausgrid/research-data-sets/distribution-zone-substation-data\n\
  \  auth: none\n  detail: >-\n    Anonymous HTTPS GET. Download tiles resolve to opaque Sitecore Content Hub URLs\n    of the form https://aopt-p-001.sitecorecontenthub.cloud/api/public/content/<guid>\n    with no key, no signature, no expiry and no terms click-through.\n- name: Ausgrid DTAPR / Unallocated Hosting Capacity ArcGIS REST FeatureServers\n  url: https://portal.data.nsw.gov.au/arcgis/rest/services/Hosted\n  auth: none\n  detail: >-\n    Anonymous ArcGIS REST query. No token parameter is required and none is accepted\n    against these layers; capabilities are \"Query\" only. NOTE the host is operated by\n    the NSW Government (portal.data.nsw.gov.au), not by Ausgrid — the DATA is\n    Ausgrid's (every record carries owner=\"Ausgrid\"), the ENDPOINT is not.\n- name: Ausgrid DTAPR data portal\n  url: https://dtapr.ausgrid.com.au/\n  auth: none\n  detail: >-\n    Anonymous Rosetta Analytics web application. Serves flat files from\n    ./ausgrid_data/ (e.g. Tech_Specification_Lines.csv,\
  \ DTAPR System Limitation\n    Template FY25.xlsx) with no key and no API.\n- name: Ausgrid outage map internal JSON routes\n  url: https://www.ausgrid.com.au/api/outages-map/\n  auth: none\n  detail: >-\n    Undocumented Next.js route handlers behind ausgrid.com.au's own outage map.\n    Anonymously reachable, no key. Not offered to developers, no published terms —\n    recorded as an observation, never as an offered API.\n- name: Customer interval meter data\n  url: https://www.ausgrid.com.au/your-energy-use/your-meter-and-supply/access-your-meter-data\n  auth: identity-verification\n  detail: >-\n    Not a credential. The requester supplies the NMI from the bill, the account\n    holder's surname or company name, the postcode and a date range; a third party\n    must attach a signed consent form from the account holder. Fulfilment is 10\n    business days for a single NMI, up to 20 for multiple, by email. There is no\n    programmatic path and no OAuth-style consent flow.\n- name: Ausgrid\
  \ Services customer sign-in\n  url: https://services.ausgrid.com.au/SignIn\n  auth: session\n  detail: Human login wall for account and connection work. No OIDC discovery document (404). Not a developer surface.\n- name: IDO connection-enquiry portal\n  url: https://idoportal.ausgrid.com.au/\n  auth: session\n  detail: >-\n    ASP.NET login wall for connection enquiries. Probes of /.well-known/openid-configuration\n    and /.well-known/oauth-authorization-server 302-redirect to a generic error page;\n    there is no discovery document.\nconsumer_data_right:\n  designated_data_holder: false\n  detail: >-\n    Ausgrid is a distribution network service provider. The CDR (Energy Sector)\n    Designation 2020 places the data-holder obligation on electricity retailers, with\n    AEMO as gateway. Ausgrid does not appear among the 84 energy brands returned by\n    https://api.cdr.gov.au/cdr-register/v1/energy/data-holders/brands/summary, so no\n    CDR OAuth 2.0 / OIDC consent stack applies to\
  \ it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ausgrid/refs/heads/main/authentication/ausgrid-authentication.yml
summary_line: 0 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Distribution Network
- Open Data
- Smart Metering
- Consumer Data Right
- Solar
- DER
- Outages
---
