---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: calibre-ebook.com
  spf: false
hosts:
- cert_expires: Jan 23 09:56:53 2027 GMT
  host: calibre-ebook.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Calibre Web Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calibre-Web, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Calibre-Web
provider_slug: calibre-web
slug: calibre-web-domain-security
source_filename: calibre-web-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calibre-ebook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 09:56:53 2027 GMT\n  hsts: false\ndomains:\n- domain: calibre-ebook.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/calibre-web/security/calibre-web-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open-Source
- eBook
- Library
- Web-App
- Python
---
