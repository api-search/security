---
api_specs:
- filename: liveramp-deliveries-api-openapi.yml
  format: yaml
  label: LiveRamp Deliveries API
  slug: liveramp-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-deliveries-api-openapi.yml
- filename: liveramp-destination-integrations-api-openapi.yml
  format: yaml
  label: LiveRamp Destination Integrations API
  slug: liveramp-destination-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-destination-integrations-api-openapi.yml
- filename: liveramp-destinations-api-openapi.yml
  format: yaml
  label: LiveRamp Destinations API
  slug: liveramp-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-destinations-api-openapi.yml
- filename: liveramp-distribution-managers-api-openapi.yml
  format: yaml
  label: LiveRamp Distribution Managers API
  slug: liveramp-distribution-managers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-distribution-managers-api-openapi.yml
- filename: liveramp-integration-connections-api-openapi.yml
  format: yaml
  label: LiveRamp Integration Connections API
  slug: liveramp-integration-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-integration-connections-api-openapi.yml
- filename: liveramp-oauth-connections-api-openapi.yml
  format: yaml
  label: LiveRamp OAuth Connections API
  slug: liveramp-oauth-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-oauth-connections-api-openapi.yml
- filename: liveramp-segment-configurations-api-openapi.yml
  format: yaml
  label: LiveRamp Segment Configurations API
  slug: liveramp-segment-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-segment-configurations-api-openapi.yml
- filename: liveramp-segments-api-openapi.yml
  format: yaml
  label: LiveRamp Segments API
  slug: liveramp-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/openapi/liveramp-segments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: liveramp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Aug 26 01:43:21 2026 GMT
  host: liveramp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 02:37:02 2026 GMT
  host: developers.liveramp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: sidecar.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liveramp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiveRamp, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LiveRamp
provider_slug: liveramp
slug: liveramp-domain-security
source_filename: liveramp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liveramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:43:21 2026 GMT\n  hsts: false\n- host: developers.liveramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 02:37:02 2026 GMT\n  hsts: false\n- host: sidecar.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: liveramp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveramp/refs/heads/main/security/liveramp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Connectivity
- Identity Resolution
- Activation
- Clean Room
- Privacy
- AdTech
---
