---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lubelogger.com
  spf: true
hosts:
- cert_expires: Nov 30 09:01:22 2026 GMT
  host: lubelogger.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lubelogger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LubeLogger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LubeLogger
provider_slug: lubelogger
slug: lubelogger-domain-security
source_filename: lubelogger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lubelogger.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 30 09:01:22 2026 GMT\n  hsts: false\ndomains:\n- domain: lubelogger.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lubelogger/security/lubelogger-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- OpenSource
- VehicleMaintenance
- FuelTracking
- SelfHosted
---
