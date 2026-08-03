---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: geckorobotics.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: cantilever.app
  spf: false
hosts:
- cert_expires: Oct 25 15:48:38 2026 GMT
  host: www.geckorobotics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 02:06:12 2026 GMT
  host: cantilever.app
  hsts: false
  https: true
  note: Cantilever customer application host; probed manually, not an apis.yml baseURL.
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:41:04 2026 GMT
  host: status.cantilever.app
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 20:30:10 2026 GMT
  host: trust.geckorobotics.com
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gecko Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gecko Robotics, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Gecko Robotics
provider_slug: gecko-robotics
slug: gecko-robotics-domain-security
source_filename: gecko-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geckorobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 15:48:38 2026 GMT\n  hsts: false\n- host: cantilever.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:06:12 2026 GMT\n  hsts: false\n  note: Cantilever customer application host; probed manually, not an apis.yml baseURL.\n- host: status.cantilever.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:41:04 2026 GMT\n- host: trust.geckorobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 20:30:10 2026 GMT\ndomains:\n- domain: geckorobotics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cantilever.app\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gecko-robotics/refs/heads/main/security/gecko-robotics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Robotics
- Artificial Intelligence
- Industrial
- Asset Management
- Infrastructure
- Inspection
- Defense
- Energy
- Manufacturing
- Predictive Maintenance
---
