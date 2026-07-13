---
api_specs:
- filename: openapi.json
  format: json
  label: LanguageTool Proofreading API
  slug: languagetool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/languagetools/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: languagetool.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: languagetoolplus.com
  spf: true
hosts:
- cert_expires: Aug 18 05:00:51 2026 GMT
  host: languagetool.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 13:21:47 2026 GMT
  host: api.languagetool.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 13:23:51 2026 GMT
  host: api.languagetoolplus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Languagetools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LanguageTool, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LanguageTool
provider_slug: languagetools
slug: languagetools-domain-security
source_filename: languagetools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: languagetool.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 05:00:51 2026 GMT\n  hsts: false\n- host: api.languagetool.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:21:47 2026 GMT\n  hsts: null\n- host: api.languagetoolplus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:23:51 2026 GMT\n  hsts: null\ndomains:\n- domain: languagetool.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: languagetoolplus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/languagetools/refs/heads/main/security/languagetools-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Grammar
- Spell Check
- Style
- Proofreading
- NLP
- Natural Language Processing
- Writing
- Open Source
---
