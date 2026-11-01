---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fleetsharp.com
  spf: true
hosts:
- cert_expires: Feb 11 17:55:35 2027 GMT
  host: fleetsharp.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fleetsharp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FleetSharp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: FleetSharp
provider_slug: fleetsharp
slug: fleetsharp-domain-security
source_filename: fleetsharp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fleetsharp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 17:55:35 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: fleetsharp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fleetsharp/security/fleetsharp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- GPS
- FleetTracking
- AssetManagement
- DashCameras
- Software
---
