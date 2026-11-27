---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Datafordeler Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datafordeler declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Datafordeler
provider_slug: datafordeler-dk
scheme_count: 4
schemes:
- description: Anonymous access (zone 0) for data the register authority publishes openly; anonymous file extracts land in a shared public folder.
  name: anonymous
  type: none
- description: Service user (tjenestebruger) with username/password in security zone 0.
  name: username-password
  type: http
- description: Certificate-based access in zone 0 and zone 5 (certservices / s5-certservices hosts) for known and approved access to protected registers such as CPR.
  name: client-certificate
  type: mutualTLS
- description: Portal (self-service) login via NemLog-in.
  name: nemlog-in
  type: openIdConnect
slug: datafordeler-dk-authentication
source_filename: datafordeler-dk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: searched\nsource: https://datafordeler.dk/vejledning/test-paa-datafordeleren/\ndocs: https://datafordeler.dk/vejledning/brugeradgang/adgangstyper/\nschemes:\n- name: anonymous\n  type: none\n  description: Anonymous access (zone 0) for data the register authority publishes openly; anonymous file extracts land in a shared public folder.\n- name: username-password\n  type: http\n  description: Service user (tjenestebruger) with username/password in security zone 0.\n- name: client-certificate\n  type: mutualTLS\n  description: Certificate-based access in zone 0 and zone 5 (certservices / s5-certservices hosts) for known and approved access to protected registers such as CPR.\n- name: nemlog-in\n  type: openIdConnect\n  description: Portal (self-service) login via NemLog-in.\n"
source_yaml_url: https://artifacts.apis.io/datafordeler-dk/authentication/datafordeler-dk-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Government
- Open Data
- Denmark
- Geospatial
- Addresses
- Property
- Registers
- GraphQL
- OGC
---
