---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: entur.org
  spf: true
hosts:
- cert_expires: Sep  9 03:39:41 2026 GMT
  host: developer.entur.org
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transport For Norway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Norway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Transport for Norway
provider_slug: transport-for-norway
slug: transport-for-norway-domain-security
source_filename: transport-for-norway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.entur.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 03:39:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: entur.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-norway/refs/heads/main/security/transport-for-norway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Transportation
- Public APIs
---
