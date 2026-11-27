---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: neodemos.nl
  spf: true
hosts:
- cert_expires: Jan  6 05:54:41 2027 GMT
  host: neodemos.nl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NeoDemos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NeoDemos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: NeoDemos
provider_slug: neodemos-nl
slug: neodemos-nl-domain-security
source_filename: neodemos-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neodemos.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 05:54:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: neodemos.nl\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/neodemos-nl/security/neodemos-nl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Civic Tech
- Transparency
- Artificial Intelligence
- Netherlands
- Government
---
