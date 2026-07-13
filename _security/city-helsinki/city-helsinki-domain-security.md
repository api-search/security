---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hri.fi
  spf: false
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: hri.fi
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: City Helsinki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City, Helsinki, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: City, Helsinki
provider_slug: city-helsinki
slug: city-helsinki-domain-security
source_filename: city-helsinki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hri.fi\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: hri.fi\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/city-helsinki/refs/heads/main/security/city-helsinki-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Government
- Public APIs
---
