---
api_specs:
- filename: calendar-api-ma-business-days-api-openapi.yml
  format: yaml
  label: API Calendrier Marocain | Jours Fériés & Ouvrables REST + SDK Python Business Days API
  slug: calendar-api-ma-business-days-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendar-api-ma/refs/heads/main/openapi/calendar-api-ma-business-days-api-openapi.yml
- filename: calendar-api-ma-holidays-api-openapi.yml
  format: yaml
  label: API Calendrier Marocain | Jours Fériés & Ouvrables REST + SDK Python Holidays API
  slug: calendar-api-ma-holidays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendar-api-ma/refs/heads/main/openapi/calendar-api-ma-holidays-api-openapi.yml
- filename: calendar-api-ma-misc-api-openapi.yml
  format: yaml
  label: API Calendrier Marocain | Jours Fériés & Ouvrables REST + SDK Python Misc API
  slug: calendar-api-ma-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendar-api-ma/refs/heads/main/openapi/calendar-api-ma-misc-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: calendar-api.ma
  spf: true
hosts:
- cert_expires: Sep 28 18:32:38 2026 GMT
  host: docs.calendar-api.ma
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 06:24:17 2026 GMT
  host: calendar-api.ma
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calendar Api Ma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API Calendrier Marocain | Jours Fériés & Ouvrables REST + SDK Python, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: API Calendrier Marocain | Jours Fériés & Ouvrables REST + SDK Python
provider_slug: calendar-api-ma
slug: calendar-api-ma-domain-security
source_filename: calendar-api-ma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.calendar-api.ma\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 18:32:38 2026 GMT\n  hsts: false\n- host: calendar-api.ma\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 06:24:17 2026 GMT\n  hsts: null\ndomains:\n- domain: calendar-api.ma\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calendar-api-ma/refs/heads/main/security/calendar-api-ma-domain-security.yml
summary_line: TLSv1.3
tags:
- holidays
- morocco
- Calendar
- business-days
- date-utilities
- data-engineering
- ETL
- python-sdk
- Localization
- reference-data
- public-holidays
- scheduling
---
