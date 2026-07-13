---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: potlatchdeltic.com
  spf: true
hosts:
- cert_expires: Aug 31 23:59:59 2026 GMT
  host: www.potlatchdeltic.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
- host: developer.potlatchdeltic.com
  https: false
- host: api.potlatchdeltic.com
  https: false
kind: domain-security
layout: security
method: probed
name: Potlatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PotlatchDeltic, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PotlatchDeltic
provider_slug: potlatch
slug: potlatch-domain-security
source_filename: potlatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.potlatchdeltic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.potlatchdeltic.com\n  https: false\n- host: api.potlatchdeltic.com\n  https: false\ndomains:\n- domain: potlatchdeltic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/potlatch/refs/heads/main/security/potlatch-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Timber
- Real Estate
- Wood Products
---
