---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com."
  - 0 issue "digicert.com"
  - 0 wild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bordeaux-metropole.fr
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: opendata.bordeaux-metropole.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transport For Bordeaux France Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Bordeaux, France, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Transport for Bordeaux, France
provider_slug: transport-for-bordeaux-france
slug: transport-for-bordeaux-france-domain-security
source_filename: transport-for-bordeaux-france-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.bordeaux-metropole.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bordeaux-metropole.fr\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com.\"\n  - 0 issue \"digicert.com\"\n  - 0 wild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-bordeaux-france/refs/heads/main/security/transport-for-bordeaux-france-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transportation
- Public APIs
---
