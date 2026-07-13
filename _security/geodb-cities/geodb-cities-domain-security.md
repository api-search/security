---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wirefreethought.com
  spf: true
hosts:
- host: geodb-cities-api.wirefreethought.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''geodb-citie'
kind: domain-security
layout: security
method: probed
name: Geodb Cities Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GeoDB Cities, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GeoDB Cities
provider_slug: geodb-cities
slug: geodb-cities-domain-security
source_filename: geodb-cities-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geodb-cities-api.wirefreethought.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''geodb-citie'\n  hsts: null\ndomains:\n- domain: wirefreethought.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geodb-cities/refs/heads/main/security/geodb-cities-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Geocoding
- Public APIs
---
