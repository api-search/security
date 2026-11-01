---
api_specs:
- filename: jackett-openapi-generated.yml
  format: yaml
  label: Jackett API
  slug: jackett-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jackett/openapi/_ae-authored/jackett-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: linuxserver.io
  spf: true
hosts:
- cert_expires: Jan 20 10:51:17 2027 GMT
  host: docs.linuxserver.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jackett Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jackett, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Jackett
provider_slug: jackett
slug: jackett-domain-security
source_filename: jackett-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.linuxserver.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 10:51:17 2027 GMT\n  hsts: false\ndomains:\n- domain: linuxserver.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/jackett/security/jackett-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- OpenSource
- Torrent
- Proxy
- API
---
