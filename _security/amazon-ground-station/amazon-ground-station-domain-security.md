---
api_specs:
- filename: amazon-ground-station-agent-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Agent API
  slug: amazon-ground-station-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-agent-api-openapi.yml
- filename: amazon-ground-station-config-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Config API
  slug: amazon-ground-station-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-config-api-openapi.yml
- filename: amazon-ground-station-contact-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Contact API
  slug: amazon-ground-station-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-contact-api-openapi.yml
- filename: amazon-ground-station-contacts-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Contacts API
  slug: amazon-ground-station-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-contacts-api-openapi.yml
- filename: amazon-ground-station-dataflowendpointgroup-api-openapi.yml
  format: yaml
  label: Amazon Ground Station DataflowEndpointGroup API
  slug: amazon-ground-station-dataflowendpointgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-dataflowendpointgroup-api-openapi.yml
- filename: amazon-ground-station-ephemerides-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Ephemerides API
  slug: amazon-ground-station-ephemerides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-ephemerides-api-openapi.yml
- filename: amazon-ground-station-ephemeris-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Ephemeris API
  slug: amazon-ground-station-ephemeris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-ephemeris-api-openapi.yml
- filename: amazon-ground-station-groundstation-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Groundstation API
  slug: amazon-ground-station-groundstation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-groundstation-api-openapi.yml
- filename: amazon-ground-station-minute-usage-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Minute Usage API
  slug: amazon-ground-station-minute-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-minute-usage-api-openapi.yml
- filename: amazon-ground-station-missionprofile-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Missionprofile API
  slug: amazon-ground-station-missionprofile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-missionprofile-api-openapi.yml
- filename: amazon-ground-station-satellite-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Satellite API
  slug: amazon-ground-station-satellite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-satellite-api-openapi.yml
- filename: amazon-ground-station-tags-api-openapi.yml
  format: yaml
  label: Amazon Ground Station Tags API
  slug: amazon-ground-station-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/openapi/amazon-ground-station-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: groundstation.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Ground Station Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Ground Station, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
slug: amazon-ground-station-domain-security
source_filename: amazon-ground-station-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: groundstation.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/security/amazon-ground-station-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
---
