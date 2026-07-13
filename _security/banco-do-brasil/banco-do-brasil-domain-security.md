---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "comodoca.com"
  - 0 issue "certisign.com.br"
  - 0 issue "certigna.com"
  - 0 iodef "mailto:ditec.redes@bb.com.br"
  - 0 issuewild "soluti.com.br"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bb.com.br
  spf: true
hosts:
- host: developers.bb.com.br
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Banco Do Brasil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Banco do Brasil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Banco do Brasil
provider_slug: banco-do-brasil
slug: banco-do-brasil-domain-security
source_filename: banco-do-brasil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.bb.com.br\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: bb.com.br\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"certisign.com.br\"\n  - 0 issue \"certigna.com\"\n  - 0 iodef \"mailto:ditec.redes@bb.com.br\"\n  - 0 issuewild \"soluti.com.br\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banco-do-brasil/refs/heads/main/security/banco-do-brasil-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Finance
- Public APIs
---
