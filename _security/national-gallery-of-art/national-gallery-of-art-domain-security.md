---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nga.gov
  spf: true
hosts:
- cert_expires: Sep 29 06:40:36 2026 GMT
  host: www.nga.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Gallery Of Art Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Gallery of Art, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Gallery of Art
provider_slug: national-gallery-of-art
slug: national-gallery-of-art-domain-security
source_filename: national-gallery-of-art-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nga.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 06:40:36 2026 GMT\n  hsts: null\ndomains:\n- domain: nga.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-gallery-of-art/refs/heads/main/security/national-gallery-of-art-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Art
- Federal Government
- Museum
- Open Data
- Cultural Heritage
---
