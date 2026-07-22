---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: factual.com
  spf: true
hosts:
- host: factual.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''factual.com'
kind: domain-security
layout: security
method: probed
name: Factual Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Factual, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Factual
provider_slug: factual
slug: factual-domain-security
source_filename: factual-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: factual.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''factual.com'\n  hsts: null\ndomains:\n- domain: factual.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/factual/refs/heads/main/security/factual-domain-security.yml
summary_line: DMARC
tags:
- Company
- Location
- Places
- Geolocation
- Points of Interest
- Location Data
- Geospatial
- Acquired
---
