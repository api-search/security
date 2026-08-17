---
api_specs:
- filename: foxglove-technologies-openapi-original.yml
  format: yaml
  label: Foxglove API
  slug: foxglove-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foxglove-technologies/refs/heads/main/openapi/foxglove-technologies-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: foxglove.dev
  spf: true
hosts:
- cert_expires: Aug 24 10:35:03 2026 GMT
  host: foxglove.dev
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 14:36:32 2026 GMT
  host: docs.foxglove.dev
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 14:26:32 2026 GMT
  host: api.foxglove.dev
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Foxglove Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foxglove Technologies, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Foxglove Technologies
provider_slug: foxglove-technologies
slug: foxglove-technologies-domain-security
source_filename: foxglove-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foxglove.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:35:03 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.foxglove.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:36:32 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api.foxglove.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 14:26:32 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: foxglove.dev\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foxglove-technologies/refs/heads/main/security/foxglove-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Observability
- Visualization
- Data Platform
- Physical AI
- Autonomy
- Fleet Management
- Developer Tools
- MCAP
- ROS
---
