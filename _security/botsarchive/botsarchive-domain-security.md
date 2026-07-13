---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: botsarchive.com
  spf: true
hosts:
- cert_expires: Aug 30 10:57:22 2026 GMT
  host: botsarchive.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Botsarchive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BotsArchive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BotsArchive
provider_slug: botsarchive
slug: botsarchive-domain-security
source_filename: botsarchive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: botsarchive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 10:57:22 2026 GMT\n  hsts: false\ndomains:\n- domain: botsarchive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botsarchive/refs/heads/main/security/botsarchive-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- Public APIs
---
