---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: charm.sh
  spf: true
hosts:
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: charm.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Charm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Charm
provider_slug: charm
slug: charm-domain-security
source_filename: charm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: charm.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: charm.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/charm/security/charm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- OpenSource
- DeveloperTools
- CLI
- Go
---
