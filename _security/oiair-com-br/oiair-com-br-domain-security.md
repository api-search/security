---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oiair.com.br
  spf: false
hosts:
- cert_expires: Dec 24 23:23:45 2026 GMT
  host: oiair.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OiAir Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OiAir, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: OiAir
provider_slug: oiair-com-br
slug: oiair-com-br-domain-security
source_filename: oiair-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oiair.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:23:45 2026 GMT\n  hsts: false\ndomains:\n- domain: oiair.com.br\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oiair-com-br/security/oiair-com-br-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
