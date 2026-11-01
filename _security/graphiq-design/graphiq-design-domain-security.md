---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: graphiq.design
  spf: false
hosts:
- cert_expires: Apr 23 23:01:05 2027 GMT
  host: graphiq.design
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Graphiq Design Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graphiq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Graphiq
provider_slug: graphiq-design
slug: graphiq-design-domain-security
source_filename: graphiq-design-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graphiq.design\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 23 23:01:05 2027 GMT\n  hsts: false\ndomains:\n- domain: graphiq.design\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/graphiq-design/security/graphiq-design-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
