---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nekretninenaprodaju.rs
  spf: false
hosts:
- cert_expires: Feb 12 15:16:07 2027 GMT
  host: nekretninenaprodaju.rs
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: nekretninenaprodaju-rs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nekretninenaprodaju-rs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: nekretninenaprodaju-rs
provider_slug: nekretninenaprodaju-rs
slug: nekretninenaprodaju-rs-domain-security
source_filename: nekretninenaprodaju-rs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nekretninenaprodaju.rs\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 15:16:07 2027 GMT\n  hsts: null\ndomains:\n- domain: nekretninenaprodaju.rs\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nekretninenaprodaju-rs/security/nekretninenaprodaju-rs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
