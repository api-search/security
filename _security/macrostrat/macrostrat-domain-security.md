---
api_specs:
- filename: macrostrat-openapi.yml
  format: yaml
  label: Macrostrat API
  slug: macrostrat
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/openapi/macrostrat-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: macrostrat.org
  spf: true
hosts:
- cert_expires: Oct  7 19:46:44 2026 GMT
  host: macrostrat.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Macrostrat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Macrostrat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Macrostrat
provider_slug: macrostrat
slug: macrostrat-domain-security
source_filename: macrostrat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: macrostrat.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:46:44 2026 GMT\n  hsts: false\ndomains:\n- domain: macrostrat.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macrostrat/refs/heads/main/security/macrostrat-domain-security.yml
summary_line: TLSv1.3
tags:
- Geological Data
- Geology
- Rocks
- Paleontology
- Earth Science
---
