---
api_specs:
- filename: epcor-outages-arcgis-openapi.yml
  format: yaml
  label: EPCOR Public Outage and Service Area Feature Services (ArcGIS REST)
  slug: epcor-outages-arcgis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epcor/refs/heads/main/openapi/epcor-outages-arcgis-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: epcor.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: savagedata.com
  note: Operator of EPCOR's Ontario Green Button portal and vendor onboarding application.
  spf: true
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:vkeymaster@esri.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arcgis.com
  note: Esri, not EPCOR. Recorded because EPCOR's only public machine-readable surface is hosted here.
  spf: true
hosts:
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: www.epcor.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: customerportal.epcor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: outages.epcor.com
  hsts: false
  https: true
  role: public outage map single page app
  tls_version: TLSv1.3
- cert_expires: Nov 17 14:06:38 2026 GMT
  epcor_controlled: false
  host: epcorgas.savagedata.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  role: Green Button Download My Data / Connect My Data customer portal (third-party operated)
  tls_version: TLSv1.2
- cert_expires: Nov 17 14:06:38 2026 GMT
  epcor_controlled: false
  host: epcorgasonboarding.savagedata.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  role: Green Button third-party vendor registration application (third-party operated)
  tls_version: TLSv1.2
- cert_expires: Oct 13 23:59:59 2026 GMT
  epcor_controlled: false
  host: services6.arcgis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  role: Esri ArcGIS Online host serving EPCOR's public feature services
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epcor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EPCOR, probed live across 6 host(s) and 3 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EPCOR
provider_slug: epcor
slug: epcor-domain-security
source_filename: epcor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  Extended beyond the two apis.yml hosts to cover every host EPCOR's programmatic surfaces actually run on -\n  the outage map, the two Green Button hosts operated for EPCOR on the Savage Data platform, and the Esri\n  ArcGIS Online host serving EPCOR's public feature services. The Green Button hosts are the weakest link:\n  TLS 1.2, a 30-day HSTS max-age, and a savagedata.com domain with no DNSSEC and no CAA - the surface that\n  carries regulated customer energy data is the least hardened of the set, and EPCOR does not control it.\nhosts:\n- host: www.epcor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: customerportal.epcor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: outages.epcor.com\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\n  role: public outage map single page app\n- host: epcorgas.savagedata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 14:06:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  role: Green Button Download My Data / Connect My Data customer portal (third-party operated)\n  epcor_controlled: false\n- host: epcorgasonboarding.savagedata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 14:06:38 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  role: Green Button third-party vendor registration application (third-party operated)\n  epcor_controlled: false\n- host: services6.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  role: Esri ArcGIS Online host serving EPCOR's public feature services\n  epcor_controlled: false\ndomains:\n- domain: epcor.com\n  dnssec: false\n  caa:\
  \ []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: savagedata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  note: Operator of EPCOR's Ontario Green Button portal and vendor onboarding application.\n- domain: arcgis.com\n  dnssec: true\n  caa: ['0 issuewild \"awstrust.com\"', '0 issuewild \"digicert.com\"', '0 iodef \"mailto:vkeymaster@esri.com\"']\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: Esri, not EPCOR. Recorded because EPCOR's only public machine-readable surface is hosted here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epcor/refs/heads/main/security/epcor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Canada
- Utilities
- Electricity
- Natural Gas
- Water
- Green Button
- Smart Metering
- Grid
- Ontario
- Alberta
- Outages
- Geospatial
- Open Data
---
