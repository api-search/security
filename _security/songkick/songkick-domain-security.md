---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: songkick.com
  spf: true
hosts:
- cert_expires: Aug 20 11:33:27 2026 GMT
  host: www.songkick.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Songkick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Songkick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Songkick
provider_slug: songkick
slug: songkick-domain-security
source_filename: songkick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.songkick.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 20 11:33:27 2026 GMT\n  hsts: false\ndomains:\n- domain: songkick.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/songkick/refs/heads/main/security/songkick-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Music
- Public APIs
---
