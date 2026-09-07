---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: adapsphotonics.com
  spf: false
hosts:
- cert_issuer: C=CN, O=GeoSSL, Inc., CN=GeoSSL DV TLS CA
  cert_not_after: '2026-12-24'
  cert_not_before: '2025-12-25'
  cert_sans:
  - '*.adapsphotonics.com'
  - adapsphotonics.com
  cert_subject: CN=*.adapsphotonics.com
  chain_length: 1
  host: www.adapsphotonics.com
  hsts: false
  http_status: 200
  https: true
  note: Origin is intermittently slow and answers 403 to repeated automated requests; probes required 30-45s timeouts and retries.
  security_headers:
    strict_transport_security: null
    x_content_type_options: nosniff
    x_frame_options: SAMEORIGIN
    x_permitted_cross_domain_policies: master-only
    x_xss_protection: 1; mode=block
  server: wts
  tls_cert_error: 'Verification fails against the Mozilla/certifi root store: the origin serves the leaf certificate only (chain_length 1) and its issuer, "GeoSSL DV TLS CA", is not present in that store. macOS/curl accepted the connection; Python with certifi did not. This is an incomplete/untrusted chain, observed 2026-09-06, not a probe failure.'
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adapsphotonics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adaps Photonics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Adaps Photonics
provider_slug: adapsphotonics
slug: adapsphotonics-domain-security
source_filename: adapsphotonics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the apis.yml website host (no API hosts exist for this company)\nhosts:\n- host: www.adapsphotonics.com\n  https: true\n  tls_version: TLSv1.3\n  http_status: 200\n  server: wts\n  cert_subject: CN=*.adapsphotonics.com\n  cert_issuer: C=CN, O=GeoSSL, Inc., CN=GeoSSL DV TLS CA\n  cert_not_before: '2025-12-25'\n  cert_not_after: '2026-12-24'\n  cert_sans:\n  - '*.adapsphotonics.com'\n  - adapsphotonics.com\n  chain_length: 1\n  tls_cert_error: >-\n    Verification fails against the Mozilla/certifi root store: the origin serves the leaf\n    certificate only (chain_length 1) and its issuer, \"GeoSSL DV TLS CA\", is not present in\n    that store. macOS/curl accepted the connection; Python with certifi did not. This is an\n    incomplete/untrusted chain, observed 2026-09-06, not a probe failure.\n  hsts: false\n  security_headers:\n    x_content_type_options: nosniff\n    x_frame_options: SAMEORIGIN\n\
  \    x_xss_protection: 1; mode=block\n    x_permitted_cross_domain_policies: master-only\n    strict_transport_security: null\n  note: >-\n    Origin is intermittently slow and answers 403 to repeated automated requests; probes\n    required 30-45s timeouts and retries.\ndomains:\n- domain: adapsphotonics.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adapsphotonics/refs/heads/main/security/adapsphotonics-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Semiconductors
- Sensors
- Photonics
- LiDAR
- 3D Sensing
- Chip Design
- Automotive
- Consumer Electronics
- Hardware
---
