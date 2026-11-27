---
api_specs:
- filename: discovergy-access-api-openapi.yml
  format: yaml
  label: inexogy Access API
  slug: discovergy-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/discovergy/openapi/discovergy-access-api-openapi.yml
- filename: discovergy-calendar-api-openapi.yml
  format: yaml
  label: inexogy Calendar API
  slug: discovergy-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/discovergy/openapi/discovergy-calendar-api-openapi.yml
- filename: discovergy-disaggregation-api-openapi.yml
  format: yaml
  label: inexogy Disaggregation API
  slug: discovergy-disaggregation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/discovergy/openapi/discovergy-disaggregation-api-openapi.yml
- filename: discovergy-loadprofile-api-openapi.yml
  format: yaml
  label: inexogy Load Profile API
  slug: discovergy-loadprofile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/discovergy/openapi/discovergy-loadprofile-api-openapi.yml
- filename: discovergy-metadata-api-openapi.yml
  format: yaml
  label: inexogy Metadata API
  slug: discovergy-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/discovergy/openapi/discovergy-metadata-api-openapi.yml
- filename: discovergy-oauth1-api-openapi.yml
  format: yaml
  label: inexogy O Auth1 API
  slug: discovergy-oauth1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/discovergy/openapi/discovergy-oauth1-api-openapi.yml
- filename: discovergy-readings-api-openapi.yml
  format: yaml
  label: inexogy Readings API
  slug: discovergy-readings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/discovergy/openapi/discovergy-readings-api-openapi.yml
- filename: discovergy-virtual-api-openapi.yml
  format: yaml
  label: inexogy Virtual API
  slug: discovergy-virtual-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/discovergy/openapi/discovergy-virtual-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: inexogy.com
  spf: true
hosts:
- cert_expires: Feb  9 17:09:20 2027 GMT
  host: www.inexogy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: inexogy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for inexogy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: inexogy
provider_slug: discovergy
slug: discovergy-domain-security
source_filename: discovergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inexogy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 17:09:20 2027 GMT\n  hsts: false\ndomains:\n- domain: inexogy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/discovergy/security/discovergy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Smart Metering
- Energy
- Data Platform
- Germany
---
