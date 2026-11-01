---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: atmo-france.org
  spf: true
hosts:
- cert_expires: Jan 23 03:47:49 2027 GMT
  host: atmo-france.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Atmo France Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atmo France, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Atmo France
provider_slug: atmo-france
slug: atmo-france-domain-security
source_filename: atmo-france-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atmo-france.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 03:47:49 2027 GMT\n  hsts: false\ndomains:\n- domain: atmo-france.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/atmo-france/security/atmo-france-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Environment
- AirQuality
- PublicService
- France
---
