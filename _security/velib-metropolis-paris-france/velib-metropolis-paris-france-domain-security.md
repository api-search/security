---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: velib-metropole.fr
  spf: true
hosts:
- cert_expires: Feb 15 13:06:35 2027 GMT
  host: www.velib-metropole.fr
  hsts: true
  hsts_max_age: 15552001
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Velib Metropolis Paris France Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Velib metropolis, Paris, France, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Velib metropolis, Paris, France
provider_slug: velib-metropolis-paris-france
slug: velib-metropolis-paris-france-domain-security
source_filename: velib-metropolis-paris-france-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.velib-metropole.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 13:06:35 2027 GMT\n  hsts: true\n  hsts_max_age: 15552001\ndomains:\n- domain: velib-metropole.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/velib-metropolis-paris-france/refs/heads/main/security/velib-metropolis-paris-france-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Transportation
- Public APIs
---
