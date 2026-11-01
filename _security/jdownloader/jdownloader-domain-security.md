---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jdownloader.org
  spf: true
hosts:
- cert_expires: Dec 26 21:06:46 2026 GMT
  host: jdownloader.org
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jdownloader Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JDownloader, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JDownloader
provider_slug: jdownloader
slug: jdownloader-domain-security
source_filename: jdownloader-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jdownloader.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 21:06:46 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: jdownloader.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/jdownloader/security/jdownloader-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Download-Manager
- File-Transfer
- Java
- Freemium
---
