---
api_specs:
- filename: terrain-openapi.yml
  format: yaml
  label: Terrain API
  slug: terrain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terrain-discovery-environment-api/refs/heads/main/openapi/terrain-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cyverse.org
  spf: true
hosts:
- cert_expires: Aug 31 13:06:27 2026 GMT
  host: cyverse.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 17:39:48 2026 GMT
  host: de.cyverse.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terrain Discovery Environment Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terrain Discovery Environment API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Terrain Discovery Environment API
provider_slug: terrain-discovery-environment-api
slug: terrain-discovery-environment-api-domain-security
source_filename: terrain-discovery-environment-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cyverse.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 13:06:27 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: de.cyverse.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 17:39:48 2026 GMT\n  hsts: null\ndomains:\n- domain: cyverse.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terrain-discovery-environment-api/refs/heads/main/security/terrain-discovery-environment-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Bioinformatics
- Data Science
- Life Sciences
- Filesystem
- Cloud Computing
- Open Source
---
