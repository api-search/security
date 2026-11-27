---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getaxionlabs.com
  spf: true
hosts:
- cert_expires: Jan 30 13:51:18 2027 GMT
  host: getaxionlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axion Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axion Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Axion Labs
provider_slug: getaxionlabs-com
slug: getaxionlabs-com-domain-security
source_filename: getaxionlabs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getaxionlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 13:51:18 2027 GMT\n  hsts: false\ndomains:\n- domain: getaxionlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/getaxionlabs-com/security/getaxionlabs-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- United Kingdom
- Studio
- Plain-English
- Tools
---
