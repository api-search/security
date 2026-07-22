---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: radiusrecycling.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: schnitzer.com
  spf: true
hosts:
- cert_expires: Aug 20 08:57:31 2026 GMT
  host: www.radiusrecycling.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: www.schnitzer.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.schnitz'
kind: domain-security
layout: security
method: probed
name: Schnitzer Steel Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schnitzer Steel Industries, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Schnitzer Steel Industries
provider_slug: schnitzer-steel-industries
slug: schnitzer-steel-industries-domain-security
source_filename: schnitzer-steel-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.radiusrecycling.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 08:57:31 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: www.schnitzer.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.schnitz'\n  hsts: null\ndomains:\n- domain: radiusrecycling.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: schnitzer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schnitzer-steel-industries/refs/heads/main/security/schnitzer-steel-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Recycling
- Steel Manufacturing
- Metals
- Circular Economy
- Fortune 500
- Scrap Metal
---
