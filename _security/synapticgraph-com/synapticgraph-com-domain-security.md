---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: synapticgraph.com
  spf: true
hosts:
- cert_expires: Jan 12 07:29:21 2027 GMT
  host: synapticgraph.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: synapticgraph-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for synapticgraph-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: synapticgraph-com
provider_slug: synapticgraph-com
slug: synapticgraph-com-domain-security
source_filename: synapticgraph-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synapticgraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 07:29:21 2027 GMT\n  hsts: null\ndomains:\n- domain: synapticgraph.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/synapticgraph-com/security/synapticgraph-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
