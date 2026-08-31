---
api_specs:
- filename: university-of-calgary-auroral-transport-model-atm-api-openapi.yml
  format: yaml
  label: University of Calgary Auroral Transport Model (ATM) API
  slug: university-of-calgary-auroral-transport-model-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-auroral-transport-model-atm-api-openapi.yml
- filename: university-of-calgary-data-distribution-api-openapi.yml
  format: yaml
  label: University of Calgary Data Distribution API
  slug: university-of-calgary-data-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-data-distribution-api-openapi.yml
- filename: university-of-calgary-hapi-api-openapi.yml
  format: yaml
  label: University of Calgary SRS HAPI (Heliophysics API) Server
  slug: university-of-calgary-hapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-hapi-api-openapi.yml
- filename: university-of-calgary-operations-sitl-api-openapi.yml
  format: yaml
  label: University of Calgary Operations - SITL API
  slug: university-of-calgary-operations-sitl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-operations-sitl-api-openapi.yml
- filename: university-of-calgary-real-time-data-api-openapi.yml
  format: yaml
  label: University of Calgary Real-Time Data API
  slug: university-of-calgary-real-time-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-real-time-data-api-openapi.yml
- filename: university-of-calgary-utilities-api-openapi.yml
  format: yaml
  label: University of Calgary Utilities API
  slug: university-of-calgary-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-utilities-api-openapi.yml
- filename: university-of-calgary-application-wadl-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Application.wadl API
  slug: university-of-calgary-application-wadl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-application-wadl-api-openapi.yml
- filename: university-of-calgary-authenticate-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Authenticate API
  slug: university-of-calgary-authenticate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-authenticate-api-openapi.yml
- filename: university-of-calgary-availability-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Availability API
  slug: university-of-calgary-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-availability-api-openapi.yml
- filename: university-of-calgary-conjunction-search-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Conjunction Search API
  slug: university-of-calgary-conjunction-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-conjunction-search-api-openapi.yml
- filename: university-of-calgary-data-products-search-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Data Products Search API
  slug: university-of-calgary-data-products-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-data-products-search-api-openapi.yml
- filename: university-of-calgary-data-sources-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Data Sources API
  slug: university-of-calgary-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-data-sources-api-openapi.yml
- filename: university-of-calgary-ephemeris-search-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Ephemeris Search API
  slug: university-of-calgary-ephemeris-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-ephemeris-search-api-openapi.yml
- filename: university-of-calgary-manage-data-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Manage Data API
  slug: university-of-calgary-manage-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-manage-data-api-openapi.yml
- filename: university-of-calgary-utils-api-openapi.yml
  format: yaml
  label: University of Calgary AuroraX Utils API
  slug: university-of-calgary-utils-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/openapi/university-of-calgary-utils-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ucalgary.ca
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: aurorax.space
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.ucalgary.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: api.phys.ucalgary.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 10:28:19 2026 GMT
  host: docs.aurorax.space
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Calgary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Calgary, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Calgary
provider_slug: university-of-calgary
slug: university-of-calgary-domain-security
source_filename: university-of-calgary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucalgary.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.phys.ucalgary.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\n- host: docs.aurorax.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:28:19 2026 GMT\n  hsts: false\ndomains:\n- domain: ucalgary.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: aurorax.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/security/university-of-calgary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Public Research University
- Canada
- Alberta
- U15
- Research
- Research Data
- Open Access
- Repository
- OAI-PMH
- Identity Federation
- Research Computing
- Space Physics
- Heliophysics
- Open Data
---
