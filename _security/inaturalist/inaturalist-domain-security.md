---
api_specs:
- filename: swagger.json
  format: json
  label: iNaturalist API v1
  slug: inaturalist-api-v1
  spec_type: OpenAPI
  url: https://api.inaturalist.org/v1/docs/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inaturalist.org
  spf: true
hosts:
- cert_expires: Aug 22 11:47:09 2026 GMT
  host: www.inaturalist.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: api.inaturalist.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Inaturalist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iNaturalist, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iNaturalist
provider_slug: inaturalist
slug: inaturalist-domain-security
source_filename: inaturalist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inaturalist.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 11:47:09 2026 GMT\n  hsts: false\n- host: api.inaturalist.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: inaturalist.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inaturalist/refs/heads/main/security/inaturalist-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Biodiversity
- Nature
- Citizen Science
- Wildlife
- Observations
- Taxa
- Ecology
---
