---
api_specs:
- filename: atco-query-api-openapi.yml
  format: yaml
  label: ATCO Query API
  slug: atco-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atco/refs/heads/main/openapi/atco-query-api-openapi.yml
- filename: atco-service-api-openapi.yml
  format: yaml
  label: ATCO Service API
  slug: atco-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atco/refs/heads/main/openapi/atco-service-api-openapi.yml
description: ''
domains:
- atco_controlled: true
  caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atco.com
  note: No DNSSEC, no CAA record, and DMARC is at p=none — monitoring only, no enforcement. All three are real gaps for a critical-infrastructure operator.
  spf: true
- atco_controlled: true
  caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:xtz8hoer@ag.dmarcian.com
  dnssec: false
  domain: atcoenergy.com
  spf: true
  spf_record: v=spf1 ip4:192.210.5.0/24 ip4:192.210.10.0/24 ip4:141.118.20.0/24 include:aspmx.pardot.com include:_spf.qualtrics.com ~all
- atco_controlled: false
  caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:vkeymaster@esri.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arcgis.com
  note: Recorded for completeness because it is the API host's registrable domain. Esri's posture is materially stronger than ATCO's — DNSSEC signed, a full CAA policy with an iodef contact, and DMARC at p=reject. This is inherited by the ATCO API, not earned by ATCO.
  operator: Esri
  spf: true
hosts:
- atco_controlled: false
  cert_expires: Oct 13 23:59:59 2026 GMT
  cors_allow_origin: '*'
  host: services7.arcgis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  operator: Esri
  role: API host (ArcGIS Online hosted feature services)
  tls_version: TLSv1.3
- atco_controlled: true
  cert_expires: Nov 15 23:59:59 2026 GMT
  host: www.atco.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  operator: ATCO
  role: corporate website
  tls_version: TLSv1.3
- atco_controlled: true
  cert_expires: Nov 15 23:59:59 2026 GMT
  host: electric.atco.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  operator: ATCO
  role: ATCO Electric — publisher of the hosting capacity map
  tls_version: TLSv1.3
- atco_controlled: true
  cert_expires: Nov 15 23:59:59 2026 GMT
  host: gas.atco.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  operator: ATCO
  role: ATCO Gas
  tls_version: TLSv1.3
- atco_controlled: true
  cert_expires: Sep 25 21:27:28 2026 GMT
  host: www.atcoenergy.com
  hsts: false
  hsts_max_age: null
  https: true
  operator: ATCO
  role: ATCO Energy — competitive Alberta retailer (Webflow-hosted)
  tls_version: TLSv1.3
- atco_controlled: partial
  cert_expires: Sep  7 14:52:11 2026 GMT
  host: store.atco.com
  hsts: false
  hsts_max_age: null
  https: true
  note: This is where a customer's own usage and billing data lives. It carries no HSTS, which is the weakest posture on the estate and sits on the most sensitive surface.
  operator: Salesforce (on ATCO's behalf)
  role: Salesforce CloudCraze customer commerce login (My Account)
  tls_version: TLSv1.3
- atco_controlled: true
  cert_expires: Sep 21 19:10:47 2026 GMT
  host: poweroutage.atco.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  operator: ATCO
  role: customer outage map (Flutter single-page app)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ATCO, probed live across 7 host(s) and 3 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ATCO
provider_slug: atco
slug: atco-domain-security
source_filename: atco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  The API host is not an ATCO domain. ATCO Electric's only public API is served from Esri's\n  shared ArcGIS Online tenant infrastructure (services7.arcgis.com), so the security posture that\n  actually protects the API belongs to Esri, while ATCO's own domains carry no API at all. Both\n  are recorded below and labelled.\nhosts:\n- host: services7.arcgis.com\n  role: API host (ArcGIS Online hosted feature services)\n  operator: Esri\n  atco_controlled: false\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  cors_allow_origin: '*'\n- host: www.atco.com\n  role: corporate website\n  operator: ATCO\n  atco_controlled: true\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: electric.atco.com\n  role: ATCO Electric —\
  \ publisher of the hosting capacity map\n  operator: ATCO\n  atco_controlled: true\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: gas.atco.com\n  role: ATCO Gas\n  operator: ATCO\n  atco_controlled: true\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: www.atcoenergy.com\n  role: ATCO Energy — competitive Alberta retailer (Webflow-hosted)\n  operator: ATCO\n  atco_controlled: true\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 21:27:28 2026 GMT\n  hsts: false\n  hsts_max_age: null\n- host: store.atco.com\n  role: Salesforce CloudCraze customer commerce login (My Account)\n  operator: Salesforce (on ATCO's behalf)\n  atco_controlled: partial\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 14:52:11 2026 GMT\n  hsts: false\n  hsts_max_age: null\n  note: >-\n    This is where a customer's own usage\
  \ and billing data lives. It carries no HSTS, which is the\n    weakest posture on the estate and sits on the most sensitive surface.\n- host: poweroutage.atco.com\n  role: customer outage map (Flutter single-page app)\n  operator: ATCO\n  atco_controlled: true\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:10:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: atco.com\n  atco_controlled: true\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: >-\n    No DNSSEC, no CAA record, and DMARC is at p=none — monitoring only, no enforcement. All three\n    are real gaps for a critical-infrastructure operator.\n- domain: atcoenergy.com\n  atco_controlled: true\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  spf_record: 'v=spf1 ip4:192.210.5.0/24 ip4:192.210.10.0/24 ip4:141.118.20.0/24 include:aspmx.pardot.com include:_spf.qualtrics.com ~all'\n  dmarc_record: 'v=DMARC1; p=none; rua=mailto:xtz8hoer@ag.dmarcian.com'\n\
  - domain: arcgis.com\n  atco_controlled: false\n  operator: Esri\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:vkeymaster@esri.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: >-\n    Recorded for completeness because it is the API host's registrable domain. Esri's posture is\n    materially stronger than ATCO's — DNSSEC signed, a full CAA policy with an iodef contact, and\n    DMARC at p=reject. This is inherited by the ATCO API, not earned by ATCO.\nsummary:\n  atco_domains_with_dnssec: 0\n  atco_domains_with_caa: 0\n  atco_domains_with_dmarc_enforcement: 0\n  atco_hosts_without_hsts: [www.atcoenergy.com, store.atco.com]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atco/refs/heads/main/security/atco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Canada
- Utilities
- Electricity
- Gas
- Grid
- Distribution
- Transmission
- DER
- Solar
- Renewables
- Open Data
- Geospatial
- Alberta
---
