---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nasa.gov
  spf: true
hosts:
- cert_expires: Aug 31 19:21:07 2026 GMT
  host: api.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 00:21:08 2026 GMT
  host: www.nasa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 03:01:39 2026 GMT
  host: eonet.gsfc.nasa.gov
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Aeronautics And Space Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The National Aeronautics and Space Administration, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: The National Aeronautics and Space Administration
provider_slug: national-aeronautics-and-space-administration
slug: national-aeronautics-and-space-administration-domain-security
source_filename: national-aeronautics-and-space-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 19:21:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 00:21:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eonet.gsfc.nasa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 03:01:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: nasa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-aeronautics-and-space-administration/refs/heads/main/security/national-aeronautics-and-space-administration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Science
- Space
- Imagery
- Earth Observation
---
