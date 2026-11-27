---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: epubtranslator.com
  spf: true
hosts:
- cert_expires: Dec 27 16:15:19 2026 GMT
  host: epubtranslator.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Epub Translator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epub Translator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Epub Translator
provider_slug: epubtranslator-com
slug: epubtranslator-com-domain-security
source_filename: epubtranslator-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: epubtranslator.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 16:15:19 2026 GMT\n  hsts: false\ndomains:\n- domain: epubtranslator.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/epubtranslator-com/security/epubtranslator-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Translation
- EPUB
- Artificial Intelligence
- eBook
---
