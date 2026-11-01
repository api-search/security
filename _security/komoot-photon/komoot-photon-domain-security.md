---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: komoot.io
  spf: false
hosts:
- cert_expires: Dec 21 20:09:58 2026 GMT
  host: photon.komoot.io
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Komoot Photon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Photon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Photon
provider_slug: komoot-photon
slug: komoot-photon-domain-security
source_filename: komoot-photon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: photon.komoot.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 21 20:09:58 2026 GMT\n  hsts: false\ndomains:\n- domain: komoot.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/komoot-photon/security/komoot-photon-domain-security.yml
summary_line: TLSv1.2
tags:
- geocoding
- openstreetmap
- search
- typeahead
- open-source
- location
---
