---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wargaming.net
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: developers.wargaming.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wargaming Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wargaming.net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wargaming.net
provider_slug: wargaming-net
slug: wargaming-net-domain-security
source_filename: wargaming-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.wargaming.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: wargaming.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wargaming-net/refs/heads/main/security/wargaming-net-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Games And Comics
- Public APIs
---
