---
api_specs:
- filename: relativity-space-openapi.yml
  format: yaml
  label: Relativity Space Terran R Launch
  slug: terran-r-launch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity-space/refs/heads/main/openapi/relativity-space-openapi.yml
- filename: relativity-space-openapi.yml
  format: yaml
  label: Relativity Space Stargate Manufacturing
  slug: stargate-manufacturing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity-space/refs/heads/main/openapi/relativity-space-openapi.yml
- filename: relativity-space-openapi.yml
  format: yaml
  label: Relativity Space Payload and Rideshare
  slug: payload-rideshare
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity-space/refs/heads/main/openapi/relativity-space-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: relativityspace.com
  spf: true
hosts:
- cert_expires: Sep  2 05:15:18 2026 GMT
  host: www.relativityspace.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Relativity Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relativity Space, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Relativity Space
provider_slug: relativity-space
slug: relativity-space-domain-security
source_filename: relativity-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.relativityspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 05:15:18 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: relativityspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relativity-space/refs/heads/main/security/relativity-space-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aerospace
- Launch Services
- Space
- Rocket
- 3D Printing
- Additive Manufacturing
---
