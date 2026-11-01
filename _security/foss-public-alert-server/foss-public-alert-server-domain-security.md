---
api_specs:
- filename: foss-public-alert-server-openapi.yaml
  format: yaml
  label: KDE API
  slug: kde-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foss-public-alert-server/openapi/foss-public-alert-server-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: kde.org
  spf: true
hosts:
- cert_expires: Dec  5 18:12:24 2026 GMT
  host: alerts.kde.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foss Public Alert Server Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FOSS Public Alert Server, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: FOSS Public Alert Server
provider_slug: foss-public-alert-server
slug: foss-public-alert-server-domain-security
source_filename: foss-public-alert-server-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alerts.kde.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 18:12:24 2026 GMT\n  hsts: null\ndomains:\n- domain: kde.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/foss-public-alert-server/security/foss-public-alert-server-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Alert
- OpenSource
- Monitoring
- Public
---
