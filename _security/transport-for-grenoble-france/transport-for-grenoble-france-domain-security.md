---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mobilites-m.fr
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: www.mobilites-m.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Transport For Grenoble France Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Grenoble, France, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Transport for Grenoble, France
provider_slug: transport-for-grenoble-france
slug: transport-for-grenoble-france-domain-security
source_filename: transport-for-grenoble-france-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mobilites-m.fr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mobilites-m.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-grenoble-france/refs/heads/main/security/transport-for-grenoble-france-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Transportation
- Public APIs
---
