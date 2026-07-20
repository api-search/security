---
api_specs:
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Projects and Plans API
  slug: dronedeploy-projects-and-plans-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Maps and Exports API
  slug: dronedeploy-maps-and-exports-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Annotations and Issues API
  slug: dronedeploy-annotations-and-issues-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Uploads and Images API
  slug: dronedeploy-uploads-and-images-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Users and Organizations API
  slug: dronedeploy-users-and-organizations-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Reports API
  slug: dronedeploy-reports-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
- filename: dronedeploy.postman_collection.json
  format: json
  label: DroneDeploy Webhooks API
  slug: dronedeploy-webhooks-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/collections/dronedeploy.postman_collection.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dronedeploy.com
  spf: true
hosts:
- cert_expires: Aug 14 03:01:05 2026 GMT
  host: www.dronedeploy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 20:44:47 2026 GMT
  host: developer-docs.dronedeploy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dronedeploy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DroneDeploy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DroneDeploy
provider_slug: dronedeploy
slug: dronedeploy-domain-security
source_filename: dronedeploy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dronedeploy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:01:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer-docs.dronedeploy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 20:44:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dronedeploy.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dronedeploy/refs/heads/main/security/dronedeploy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Drone Mapping
- Reality Capture
- Aerial Analytics
- Geospatial
- GraphQL
- Photogrammetry
---
