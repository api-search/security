---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trustpointgps.com
  spf: true
hosts:
- cert_expires: Aug 13 17:52:05 2026 GMT
  host: trustpointgps.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trustpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrustPoint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TrustPoint
provider_slug: trustpoint
slug: trustpoint-domain-security
source_filename: trustpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trustpointgps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 17:52:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: trustpointgps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustpoint/refs/heads/main/security/trustpoint-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- GNSS
- Satellites
- Navigation
- Positioning
- Timing
- PNT
- Space
- Aerospace
---
