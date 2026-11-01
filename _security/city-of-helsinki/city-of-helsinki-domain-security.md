---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hel.fi
  spf: true
hosts:
- cert_expires: Mar 19 11:21:51 2027 GMT
  host: www.hel.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: City Of Helsinki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City of Helsinki, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: City of Helsinki
provider_slug: city-of-helsinki
slug: city-of-helsinki-domain-security
source_filename: city-of-helsinki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hel.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 11:21:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hel.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/city-of-helsinki/security/city-of-helsinki-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- OpenData
- Finland
- Helsinki
- CivicTech
- PublicServices
---
