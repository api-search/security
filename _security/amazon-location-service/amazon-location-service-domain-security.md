---
api_specs:
- filename: amazon-location-service-maps-api-openapi.yml
  format: yaml
  label: Amazon Location Service Maps API
  slug: amazon-location-service-maps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-maps-api-openapi.yml
- filename: amazon-location-service-geofencing-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Geofencing API
  slug: amazon-location-service-geofencing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-geofencing-api-openapi.yml
- filename: amazon-location-service-metadata-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Metadata API
  slug: amazon-location-service-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-metadata-api-openapi.yml
- filename: amazon-location-service-operations-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Operations API
  slug: amazon-location-service-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-operations-api-openapi.yml
- filename: amazon-location-service-places-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Places API
  slug: amazon-location-service-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-places-api-openapi.yml
- filename: amazon-location-service-positions-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Positions API
  slug: amazon-location-service-positions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-positions-api-openapi.yml
- filename: amazon-location-service-routes-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Routes API
  slug: amazon-location-service-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-routes-api-openapi.yml
- filename: amazon-location-service-tags-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Tags API
  slug: amazon-location-service-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-tags-api-openapi.yml
- filename: amazon-location-service-tracking-api-openapi.yml
  format: yaml
  label: Amazon Location Service Location Service Tracking API
  slug: amazon-location-service-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-location-service/openapi/amazon-location-service-tracking-api-openapi.yml
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
- host: geo.amazonaws.com
  https: false
- host: geo.us-east-1.amazonaws.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Amazon Location Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Location Service, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Location Service
provider_slug: amazon-location-service
slug: amazon-location-service-domain-security
source_filename: amazon-location-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: geo.amazonaws.com\n  https: false\n- host: geo.us-east-1.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-location-service/security/amazon-location-service-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geocoding
- Geofencing
- Location
- Maps
- Routing
---
