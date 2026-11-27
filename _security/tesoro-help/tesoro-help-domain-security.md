---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tesoro.help
  spf: false
hosts:
- cert_expires: Jan 19 00:13:39 2027 GMT
  host: tesoro.help
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: tesoro-help Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tesoro-help, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: tesoro-help
provider_slug: tesoro-help
slug: tesoro-help-domain-security
source_filename: tesoro-help-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tesoro.help\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 00:13:39 2027 GMT\n  hsts: false\ndomains:\n- domain: tesoro.help\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tesoro-help/security/tesoro-help-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
