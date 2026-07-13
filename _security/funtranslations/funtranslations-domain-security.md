---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: funtranslations.com
  spf: false
hosts:
- cert_expires: Sep  2 23:57:18 2026 GMT
  host: api.funtranslations.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Funtranslations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FunTranslations, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FunTranslations
provider_slug: funtranslations
slug: funtranslations-domain-security
source_filename: funtranslations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.funtranslations.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 23:57:18 2026 GMT\n  hsts: null\ndomains:\n- domain: funtranslations.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/funtranslations/refs/heads/main/security/funtranslations-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
