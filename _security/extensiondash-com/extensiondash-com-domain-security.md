---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: extensiondash.com
  spf: true
hosts:
- cert_expires: Jan 19 07:19:07 2027 GMT
  host: extensiondash.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ExtensionDash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ExtensionDash, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ExtensionDash
provider_slug: extensiondash-com
slug: extensiondash-com-domain-security
source_filename: extensiondash-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: extensiondash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 07:19:07 2027 GMT\n  hsts: false\ndomains:\n- domain: extensiondash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/extensiondash-com/security/extensiondash-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SEO
- Browser Extension
- Market Intelligence
- AI Integration
- Analytics
---
