---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wikimapia.org
  spf: true
hosts:
- cert_expires: Oct  3 07:34:55 2026 GMT
  host: wikimapia.org
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  3 07:34:55 2026 GMT
  host: api.wikimapia.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Wikimapia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wikimapia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Wikimapia
provider_slug: wikimapia
slug: wikimapia-domain-security
source_filename: wikimapia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wikimapia.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 07:34:55 2026 GMT\n  hsts: false\n- host: api.wikimapia.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 07:34:55 2026 GMT\n  hsts: false\ndomains:\n- domain: wikimapia.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikimapia/refs/heads/main/security/wikimapia-domain-security.yml
summary_line: TLSv1.2
tags:
- Geospatial
- Mapping
- Crowdsourced
- Places
- Geographic Data
---
