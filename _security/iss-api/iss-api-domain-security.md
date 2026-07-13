---
api_specs:
- filename: iss_location.html
  format: yaml
  label: ISS Current Location
  slug: iss-location-now
  spec_type: OpenAPI
  url: https://open-notify-api.readthedocs.io/en/latest/iss_location.html
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: open-notify.org
  spf: false
hosts:
- host: open-notify.org
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''open-notify'
- host: api.open-notify.org
  https: false
kind: domain-security
layout: security
method: probed
name: Iss Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ISS Location API (Open Notify), probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ISS Location API (Open Notify)
provider_slug: iss-api
slug: iss-api-domain-security
source_filename: iss-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open-notify.org\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''open-notify'\n  hsts: null\n- host: api.open-notify.org\n  https: false\ndomains:\n- domain: open-notify.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iss-api/refs/heads/main/security/iss-api-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Space
- ISS
- International Space Station
- NASA
- Location
- Geolocation
- Astronauts
- Real-Time
- Open Source
- Public API
- Free
---
