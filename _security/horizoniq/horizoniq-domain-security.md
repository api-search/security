---
api_specs:
- filename: horizoniq-compass-openapi-original.yml
  format: yaml
  label: HorizonIQ Compass API
  slug: horizoniq-compass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/openapi/horizoniq-compass-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: horizoniq.com
  spf: true
hosts:
- cert_expires: Sep 23 12:38:06 2026 GMT
  host: www.horizoniq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Horizoniq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HorizonIQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HorizonIQ
provider_slug: horizoniq
slug: horizoniq-domain-security
source_filename: horizoniq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.horizoniq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 12:38:06 2026 GMT\n  hsts: false\ndomains:\n- domain: horizoniq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizoniq/refs/heads/main/security/horizoniq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Cloud
- Bare Metal
- Infrastructure
- Private Cloud
- Hosting
- Data Center
- Compute
- Storage
---
