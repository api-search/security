---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ratp.fr
  spf: true
hosts:
- cert_expires: Aug 19 10:15:34 2026 GMT
  host: data.ratp.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transport For Paris France Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Paris, France, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Transport for Paris, France
provider_slug: transport-for-paris-france
slug: transport-for-paris-france-domain-security
source_filename: transport-for-paris-france-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.ratp.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 10:15:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ratp.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-paris-france/refs/heads/main/security/transport-for-paris-france-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transportation
- Public APIs
---
