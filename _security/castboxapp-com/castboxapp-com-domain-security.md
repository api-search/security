---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: castbox.fm
  spf: true
hosts:
- cert_expires: Jan 19 08:44:14 2027 GMT
  host: castbox.fm
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Castboxapp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for castboxapp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: castboxapp
provider_slug: castboxapp-com
slug: castboxapp-com-domain-security
source_filename: castboxapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: castbox.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 08:44:14 2027 GMT\n  hsts: false\ndomains:\n- domain: castbox.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/castboxapp-com/security/castboxapp-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
