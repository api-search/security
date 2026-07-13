---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: metrolisboa.pt
  spf: true
hosts:
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: app.metrolisboa.pt
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metro Lisboa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metro Lisboa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Metro Lisboa
provider_slug: metro-lisboa
slug: metro-lisboa-domain-security
source_filename: metro-lisboa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.metrolisboa.pt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: metrolisboa.pt\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metro-lisboa/refs/heads/main/security/metro-lisboa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Public APIs
---
