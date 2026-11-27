---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: searxng.org
  spf: true
hosts:
- cert_expires: Jan 26 14:10:22 2027 GMT
  host: searxng.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SearXNG Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SearXNG, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SearXNG
provider_slug: searxng
slug: searxng-domain-security
source_filename: searxng-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: searxng.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 14:10:22 2027 GMT\n  hsts: false\ndomains:\n- domain: searxng.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/searxng/security/searxng-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Search
- Privacy
- Open Source
- Metasearch
- Decentralization
---
