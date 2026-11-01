---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: libre.fm
  spf: true
hosts:
- cert_expires: Jan  6 18:27:28 2027 GMT
  host: libre.fm
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Libre Fm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Libre.fm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Libre.fm
provider_slug: libre-fm
slug: libre-fm-domain-security
source_filename: libre-fm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: libre.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 18:27:28 2027 GMT\n  hsts: false\ndomains:\n- domain: libre.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/libre-fm/security/libre-fm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Music
- Open-Source
- Scrobbling
- Community
---
