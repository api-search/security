---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bhphotovideo.com
  spf: true
hosts:
- cert_expires: Jan 23 10:55:09 2027 GMT
  host: bhphotovideo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: B&H Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for B&H, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: B&H
provider_slug: b-h-photo-video
slug: b-h-photo-video-domain-security
source_filename: b-h-photo-video-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bhphotovideo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 10:55:09 2027 GMT\n  hsts: null\ndomains:\n- domain: bhphotovideo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/b-h-photo-video/security/b-h-photo-video-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
