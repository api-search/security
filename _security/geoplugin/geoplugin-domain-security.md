---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: geoplugin.com
  spf: true
hosts:
- cert_expires: Sep 13 23:49:22 2026 GMT
  host: www.geoplugin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geoplugin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for geoPlugin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: geoPlugin
provider_slug: geoplugin
slug: geoplugin-domain-security
source_filename: geoplugin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geoplugin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:49:22 2026 GMT\n  hsts: false\ndomains:\n- domain: geoplugin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geoplugin/refs/heads/main/security/geoplugin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geocoding
- Public APIs
---
