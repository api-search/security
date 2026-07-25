---
api_specs:
- filename: labvantage-containers-api-openapi.yml
  format: yaml
  label: LabVantage Solutions Containers API
  slug: labvantage-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/labvantage/refs/heads/main/openapi/labvantage-containers-api-openapi.yml
- filename: labvantage-instruments-api-openapi.yml
  format: yaml
  label: LabVantage Solutions Instruments API
  slug: labvantage-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/labvantage/refs/heads/main/openapi/labvantage-instruments-api-openapi.yml
- filename: labvantage-results-api-openapi.yml
  format: yaml
  label: LabVantage Solutions Results API
  slug: labvantage-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/labvantage/refs/heads/main/openapi/labvantage-results-api-openapi.yml
- filename: labvantage-samples-api-openapi.yml
  format: yaml
  label: LabVantage Solutions Samples API
  slug: labvantage-samples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/labvantage/refs/heads/main/openapi/labvantage-samples-api-openapi.yml
- filename: labvantage-tests-api-openapi.yml
  format: yaml
  label: LabVantage Solutions Tests API
  slug: labvantage-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/labvantage/refs/heads/main/openapi/labvantage-tests-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: labvantage.com
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.labvantage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Labvantage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LabVantage Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LabVantage Solutions
provider_slug: labvantage
slug: labvantage-domain-security
source_filename: labvantage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.labvantage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: labvantage.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/labvantage/refs/heads/main/security/labvantage-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pharma
- Laboratory
- LIMS
- Quality
- GxP
---
