---
api_specs:
- filename: syncthing-openapi-generated.yml
  format: yaml
  label: Syncthing API
  slug: syncthing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/syncthing/openapi/_ae-authored/syncthing-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: syncthing.net
  spf: true
hosts:
- cert_expires: Nov 29 04:02:23 2026 GMT
  host: syncthing.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Syncthing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syncthing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Syncthing
provider_slug: syncthing
slug: syncthing-domain-security
source_filename: syncthing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syncthing.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 04:02:23 2026 GMT\n  hsts: false\ndomains:\n- domain: syncthing.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/syncthing/security/syncthing-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- File Synchronization
- Open Source
- Cross-Platform
- Encryption
- Peer-to-Peer
---
