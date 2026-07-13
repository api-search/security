---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iucnredlist.org
  spf: true
hosts:
- cert_expires: Sep 24 14:42:10 2026 GMT
  host: apiv3.iucnredlist.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iucn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IUCN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IUCN
provider_slug: iucn
slug: iucn-domain-security
source_filename: iucn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiv3.iucnredlist.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 14:42:10 2026 GMT\n  hsts: null\ndomains:\n- domain: iucnredlist.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iucn/refs/heads/main/security/iucn-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Animals
- Public APIs
---
