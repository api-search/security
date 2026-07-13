---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gob.mx
  spf: true
hosts:
- host: datos.gob.mx
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Open Government Mexico Datos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Mexico, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Open Government, Mexico
provider_slug: open-government-mexico-datos
slug: open-government-mexico-datos-domain-security
source_filename: open-government-mexico-datos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datos.gob.mx\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: gob.mx\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-mexico-datos/refs/heads/main/security/open-government-mexico-datos-domain-security.yml
summary_line: DNSSEC
tags:
- Government
- Public APIs
---
