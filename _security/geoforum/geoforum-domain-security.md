---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: geoforum.dk
  spf: true
hosts:
- cert_expires: Jan  2 12:03:45 2027 GMT
  host: geoforum.dk
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Geoforum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geoforum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Geoforum
provider_slug: geoforum
slug: geoforum-domain-security
source_filename: geoforum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geoforum.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 12:03:45 2027 GMT\n  hsts: false\ndomains:\n- domain: geoforum.dk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/geoforum/security/geoforum-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
