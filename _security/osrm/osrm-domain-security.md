---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: project-osrm.org
  spf: true
hosts:
- cert_expires: Jan  6 00:58:52 2027 GMT
  host: project-osrm.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Osrm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OSRM (Project OSRM, self-hosted), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OSRM (Project OSRM, self-hosted)
provider_slug: osrm
slug: osrm-domain-security
source_filename: osrm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: project-osrm.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 00:58:52 2027 GMT\n  hsts: false\ndomains:\n- domain: project-osrm.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/osrm/security/osrm-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Routing
- OpenSource
- Navigation
- GIS
---
