---
api_specs:
- filename: spec
  format: yaml
  label: LibreTranslate API
  slug: libre-translate-api
  spec_type: OpenAPI
  url: https://libretranslate.com/spec
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: libretranslate.com
  spf: true
hosts:
- cert_expires: Sep 17 12:07:55 2026 GMT
  host: libretranslate.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Libre Translate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LibreTranslate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LibreTranslate
provider_slug: libre-translate
slug: libre-translate-domain-security
source_filename: libre-translate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: libretranslate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 12:07:55 2026 GMT\n  hsts: false\ndomains:\n- domain: libretranslate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/libre-translate/refs/heads/main/security/libre-translate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Translation
- Machine Translation
- Natural Language Processing
- Open Source
- Self-Hosted
---
