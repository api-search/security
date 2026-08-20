---
api_specs:
- filename: flock-safety-alerts-api-openapi.yml
  format: yaml
  label: Flock Safety Alerts API
  slug: flock-safety-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-alerts-api-openapi.yml
- filename: flock-safety-cad-events-api-openapi.yml
  format: yaml
  label: Flock Safety CAD Events API
  slug: flock-safety-cad-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-cad-events-api-openapi.yml
- filename: flock-safety-custom-hotlists-api-openapi.yml
  format: yaml
  label: Flock Safety Custom Hotlists API
  slug: flock-safety-custom-hotlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-custom-hotlists-api-openapi.yml
- filename: flock-safety-devices-api-openapi.yml
  format: yaml
  label: Flock Safety Devices API
  slug: flock-safety-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-devices-api-openapi.yml
- filename: flock-safety-lpr-hotlist-alert-subscriptions-api-openapi.yml
  format: yaml
  label: Flock Safety LPR Hotlist Alert Subscriptions API
  slug: flock-safety-lpr-hotlist-alert-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-lpr-hotlist-alert-subscriptions-api-openapi.yml
- filename: flock-safety-oauth2-api-openapi.yml
  format: yaml
  label: Flock Safety OAuth2 API
  slug: flock-safety-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-oauth2-api-openapi.yml
- filename: flock-safety-plate-reads-api-openapi.yml
  format: yaml
  label: Flock Safety Plate Reads API
  slug: flock-safety-plate-reads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-plate-reads-api-openapi.yml
- filename: flock-safety-tracked-subject-types-api-openapi.yml
  format: yaml
  label: Flock Safety Tracked Subject Types API
  slug: flock-safety-tracked-subject-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-tracked-subject-types-api-openapi.yml
- filename: flock-safety-tracked-subjects-api-openapi.yml
  format: yaml
  label: Flock Safety Tracked Subjects API
  slug: flock-safety-tracked-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-tracked-subjects-api-openapi.yml
- filename: flock-safety-vehicle-images-api-openapi.yml
  format: yaml
  label: Flock Safety Vehicle Images API
  slug: flock-safety-vehicle-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/openapi/flock-safety-vehicle-images-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: flocksafety.com
  spf: true
hosts:
- cert_expires: Oct 14 20:46:22 2026 GMT
  host: flocksafety.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 01:19:34 2026 GMT
  host: docs.flocksafety.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 21:25:32 2026 GMT
  host: api.flocksafety.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flock Safety Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flock Safety, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Flock Safety
provider_slug: flock-safety
slug: flock-safety-domain-security
source_filename: flock-safety-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flocksafety.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 20:46:22 2026 GMT\n  hsts: false\n- host: docs.flocksafety.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 01:19:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.flocksafety.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 21:25:32 2026 GMT\n  hsts: null\ndomains:\n- domain: flocksafety.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flock-safety/refs/heads/main/security/flock-safety-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- American Dynamism
- Public Safety
- Law Enforcement
- License Plate Recognition
- LPR
- Physical Security
- Surveillance
- Computer-Vision
- Webhook
- Geolocation
- CAD
---
