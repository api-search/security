---
api_specs:
- filename: openfema-fire-data-openapi.yml
  format: yaml
  label: OpenFEMA Fire Data API
  slug: openfema-fire-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-fire-administration/refs/heads/main/openapi/openfema-fire-data-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fema.gov
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.fema.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: United States Fire Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United States Fire Administration, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: United States Fire Administration
provider_slug: united-states-fire-administration
slug: united-states-fire-administration-domain-security
source_filename: united-states-fire-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fema.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fema.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-fire-administration/refs/heads/main/security/united-states-fire-administration-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Fire Safety
- Emergency Management
- Public Safety
- FEMA
---
