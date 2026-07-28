---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Canada Energy Regulator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Canada Energy Regulator secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Canada Energy Regulator
provider_slug: canada-energy-regulator
scheme_count: 0
schemes: []
slug: canada-energy-regulator-authentication
source_filename: canada-energy-regulator-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: live anonymous probes of every Canada Energy Regulator machine-readable surface, 2026-07-27\ndocs: https://www.cer-rec.gc.ca/en/about/open-government/\nnote: 'There is no OpenAPI on any CER host, so this profile was not derived from securitySchemes — it was established\n  by probing each surface anonymously and recording what it accepted. The finding is that the Canada Energy Regulator\n  requires no authentication anywhere on its public data estate: no API key, no OAuth, no OIDC, no mTLS, no bearer\n  token was required or even offered. Access control is by open licence (OGL-Canada), not by credential.'\nsummary:\n  types:\n  - none\n  anonymous: true\n  api_key_in: []\n  oauth2_flows: []\n  registration_required: false\n  terms_click_through: false\nschemes: []\nsurfaces:\n- name: CER ArcGIS Online feature services\n  base: https://services5.arcgis.com/vNzamREXvX2WcX6d/arcgis/rest/services\n  auth: none\n  verified: '2026-07-27'\n\
  \  evidence: GET /Incident_Data_English_20191007_View/FeatureServer/0/query?where=1=1&returnCountOnly=true&f=json returned\n    {\"count\":1899} with no credential.\n- name: CER Assessments on the Federal Geospatial Platform\n  base: https://maps-cartes.services.geo.ca/server_serveur/rest/services/NRCan/CER_Assessments_EN/MapServer\n  auth: none\n  verified: '2026-07-27'\n  evidence: MapServer ?f=json returned 200/3,005 bytes and WMS 1.3.0 GetCapabilities returned 200/7,019 bytes of valid\n    XML, both anonymous.\n- name: Open Government Portal CKAN Action API (operated by Treasury Board Secretariat, not the CER)\n  base: https://open.canada.ca/data/api/3/action\n  auth: none\n  verified: '2026-07-27'\n  evidence: GET /package_search?fq=owner_org:A3EE9522-882F-47B0-BA7D-83420DC8577C returned 83 datasets anonymously.\n  caveat: A WAF in front of open.canada.ca rejects requests without a browser-like User-Agent, returning an HTML \"Request\n    Rejected\" body under HTTP 200. This is not\
  \ authentication, but it silently breaks naive clients and is the single\n    most likely cause of a failed first integration.\n- name: CER bulk CSV tree\n  base: https://www.cer-rec.gc.ca/open/\n  auth: none\n  verified: '2026-07-27'\n  evidence: A 10,110-byte LNG exports CSV was downloaded anonymously. The directory itself is not browsable (soft\n    403 body under HTTP 200); individual file paths resolve.\ncredentialed_systems_not_apis:\n- name: REGDOCS\n  url: https://apps.cer-rec.gc.ca/REGDOCS/Home/Index\n  http_status: 200\n  note: Public regulatory document search UI. Browsable without login; no documented API and no machine authentication.\n- name: Event Reporting System (ERS)\n  url: https://apps.cer-rec.gc.ca/ERS/\n  http_status: 200\n  note: Inbound incident reporting for regulated companies. HTML session login for filers; no documented API auth.\n    Its output is republished as the open Incidents dataset.\ndiscovery_probes:\n- url: https://www.cer-rec.gc.ca/.well-known/openid-configuration\n\
  \  http_status: 200\n  result: soft 404 — 4,405-byte CER HTML error page. No OIDC discovery document.\n- url: https://www.cer-rec.gc.ca/.well-known/oauth-authorization-server\n  http_status: 200\n  result: soft 404, same page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canada-energy-regulator/refs/heads/main/authentication/canada-energy-regulator-authentication.yml
summary_line: none · 0 schemes
tags:
- Energy
- Canada
- Regulation
- Government
- Pipelines
- Electricity
- Natural Gas
- Crude Oil
- Energy Markets
- Open Data
- Geospatial
---
