---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: xteve.de
  spf: true
hosts:
- host: xteve.de
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1127)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xteve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for xTeVe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: xTeVe
provider_slug: xteve
slug: xteve-domain-security
source_filename: xteve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xteve.de\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1127)'\n  hsts: null\ndomains:\n- domain: xteve.de\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/xteve/security/xteve-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Media
- IPTV
- OpenSource
- Proxy
- Plex
- Emby
---
