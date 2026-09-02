---
api_specs:
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP API
  slug: nexxen-dsp-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP Token Service
  slug: nexxen-dsp-token-service
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP Reporting API
  slug: nexxen-dsp-reporting-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP Device API
  slug: nexxen-dsp-device-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
- filename: tremor-video.postman_collection.json
  format: json
  label: Nexxen DSP Location API
  slug: nexxen-dsp-location-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/collections/tremor-video.postman_collection.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nexxen.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: postman.com
  spf: true
hosts:
- cert_expires: Sep 22 12:29:30 2026 GMT
  host: nexxen.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 09:01:44 2026 GMT
  host: www.postman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: services.amobee.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15724800
  hsts_note: 'The automated probe records null because the host root returns a bare 404 with no HSTS. On a real API path the gateway does send it — observed 2026-08-13 on GET https://services.amobee.com/campaign/v5/api/advertisers (401): "strict-transport-security: max-age=15724800; includeSubDomains".'
  https: true
  security_headers_observed:
  - x-content-type-options: nosniff
  - x-frame-options: SAMEORIGIN
  - referrer-policy: strict-origin
  - content-security-policy: present
  - permissions-policy: present
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tremor Video Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tremor Video, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tremor Video
provider_slug: tremor-video
slug: tremor-video-domain-security
source_filename: tremor-video-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexxen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 12:29:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.postman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 09:01:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.amobee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n  hsts_include_subdomains: true\n  hsts_note: >-\n    The automated probe records null because the host root returns a bare 404 with no HSTS. On a\n    real API path the gateway does send it — observed 2026-08-13 on\n    GET https://services.amobee.com/campaign/v5/api/advertisers (401):\n    \"strict-transport-security: max-age=15724800; includeSubDomains\".\n  security_headers_observed:\n  - x-content-type-options: nosniff\n  - x-frame-options:\
  \ SAMEORIGIN\n  - referrer-policy: strict-origin\n  - content-security-policy: present\n  - permissions-policy: present\ndomains:\n- domain: nexxen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: postman.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tremor-video/refs/heads/main/security/tremor-video-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MarTech
- Advertising
- AdTech
- DSP
- Programmatic
- CTV
- Video Advertising
---
