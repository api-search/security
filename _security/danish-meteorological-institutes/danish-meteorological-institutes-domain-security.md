---
api_specs:
- filename: dmi-open-data-api-openapi.yml
  format: yaml
  label: DMI Open Data API
  slug: dmi-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/danish-meteorological-institutes/refs/heads/main/openapi/dmi-open-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dmi.dk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: govcloud.dk
  spf: true
hosts:
- cert_expires: Sep  7 07:31:50 2026 GMT
  host: www.dmi.dk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 05:51:26 2026 GMT
  host: opendatadocs.dmi.govcloud.dk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: opendataapi.dmi.dk
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Danish Meteorological Institutes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Danish Meteorological Institutes, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Danish Meteorological Institutes
provider_slug: danish-meteorological-institutes
slug: danish-meteorological-institutes-domain-security
source_filename: danish-meteorological-institutes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dmi.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 07:31:50 2026 GMT\n  hsts: false\n- host: opendatadocs.dmi.govcloud.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:51:26 2026 GMT\n  hsts: null\n- host: opendataapi.dmi.dk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dmi.dk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: govcloud.dk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/danish-meteorological-institutes/refs/heads/main/security/danish-meteorological-institutes-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Climate
- Environment
- Lightning
- Meteorological
- Ocean
- Open Data
- Weather
---
