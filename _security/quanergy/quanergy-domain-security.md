---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quanergy.com
  mx: Google Workspace (aspmx.l.google.com)
  nameservers:
  - ns43.domaincontrol.com
  - ns44.domaincontrol.com
  spf: true
hosts:
- cert_expires: Oct 10 06:59:40 2026 GMT
  host: quanergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
  x-note: Fronted by Sucuri/Cloudproxy; sends CSP upgrade-insecure-requests, X-Frame-Options SAMEORIGIN, X-Content-Type-Options nosniff, but no Strict-Transport-Security.
- cert_expires: Sep 30 23:59:59 2026 GMT
  cert_verify: 0 (ok)
  host: downloads.quanergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
  x-note: AWS CloudFront (d37kvolyxq2d8.cloudfront.net). Hosts the public QORTEX DTC API Reference, user guides and installers; probed 2026-08-05.
kind: domain-security
layout: security
method: probed
name: Quanergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quanergy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Quanergy
provider_slug: quanergy
slug: quanergy-domain-security
source_filename: quanergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quanergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:59:40 2026 GMT\n  hsts: false\n  x-note: 'Fronted by Sucuri/Cloudproxy; sends CSP upgrade-insecure-requests, X-Frame-Options\n    SAMEORIGIN, X-Content-Type-Options nosniff, but no Strict-Transport-Security.'\n- host: downloads.quanergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  cert_verify: 0 (ok)\n  hsts: false\n  x-note: 'AWS CloudFront (d37kvolyxq2d8.cloudfront.net). Hosts the public QORTEX DTC API\n    Reference, user guides and installers; probed 2026-08-05.'\ndomains:\n- domain: quanergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  nameservers: [ns43.domaincontrol.com, ns44.domaincontrol.com]\n  mx: Google Workspace (aspmx.l.google.com)\ngaps:\n- No HSTS on either host.\n- No DNSSEC and\
  \ no CAA records on quanergy.com.\n- 'No /.well-known/security.txt (RFC 9116) — probed 2026-08-05, HTTP 404.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quanergy/refs/heads/main/security/quanergy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- LiDAR
- Sensors
- Physical Security
- Perimeter Security
- Perception
- Crowd Management
- Industrial Automation
- Internet of Things
- gRPC
- Streaming
- Hardware
---
