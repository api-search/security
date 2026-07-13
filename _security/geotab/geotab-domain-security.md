---
api_specs:
- filename: geotab-data-intake-gateway-openapi.yml
  format: yaml
  label: Data Intake Gateway API
  slug: data-intake-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geotab/refs/heads/main/openapi/geotab-data-intake-gateway-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:it@geotab.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: geotab.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.geotab.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: developers.geotab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: my.geotab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geotab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geotab, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Geotab
provider_slug: geotab
slug: geotab-domain-security
source_filename: geotab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geotab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: developers.geotab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.geotab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: geotab.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:it@geotab.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geotab/refs/heads/main/security/geotab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fleet Management
- Telematics
- Vehicle Tracking
- ELD Compliance
- Driver Behavior
- Fuel Monitoring
- Route Optimization
- GPS Tracking
- IoT
---
