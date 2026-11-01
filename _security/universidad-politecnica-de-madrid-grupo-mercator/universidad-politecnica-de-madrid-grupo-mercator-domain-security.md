---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: latingeo.net
  spf: false
hosts:
- host: www.latingeo.net
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.latinge'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Universidad Politecnica De Madrid Grupo Mercator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universidad Politecnica de Madrid (Grupo Mercator), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Universidad Politecnica de Madrid (Grupo Mercator)
provider_slug: universidad-politecnica-de-madrid-grupo-mercator
slug: universidad-politecnica-de-madrid-grupo-mercator-domain-security
source_filename: universidad-politecnica-de-madrid-grupo-mercator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.latingeo.net\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.latinge'\n  hsts: null\ndomains:\n- domain: latingeo.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/universidad-politecnica-de-madrid-grupo-mercator/security/universidad-politecnica-de-madrid-grupo-mercator-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
