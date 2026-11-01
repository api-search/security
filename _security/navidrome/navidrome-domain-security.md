---
api_specs:
- filename: navidrome-server-api-openapi.yml
  format: yaml
  label: Navidrome Server API
  slug: navidrome-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/navidrome/openapi/navidrome-server-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: navidrome.org
  spf: true
hosts:
- cert_expires: Dec  5 21:17:00 2026 GMT
  host: navidrome.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Navidrome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Navidrome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Navidrome
provider_slug: navidrome
slug: navidrome-domain-security
source_filename: navidrome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: navidrome.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 21:17:00 2026 GMT\n  hsts: false\ndomains:\n- domain: navidrome.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/navidrome/security/navidrome-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Music
- Streaming
- Self-Hosted
- Open-Source
- Media-Server
---
