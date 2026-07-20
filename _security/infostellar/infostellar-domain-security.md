---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: infostellar.net
  spf: false
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazontrust.com"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: true
  domain: stellarstation.com
  spf: true
hosts:
- cert_expires: Oct  7 06:23:27 2026 GMT
  host: www.infostellar.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 11:38:16 2026 GMT
  host: api.stellarstation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infostellar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infostellar, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Infostellar
provider_slug: infostellar
slug: infostellar-domain-security
source_filename: infostellar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infostellar.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 06:23:27 2026 GMT\n  hsts: false\n- host: api.stellarstation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 11:38:16 2026 GMT\n  hsts: false\ndomains:\n- domain: infostellar.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: stellarstation.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infostellar/refs/heads/main/security/infostellar-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Space
- Satellite
- Ground Station
- Aerospace
- Telemetry
- gRPC
- GSaaS
- Orbital
---
