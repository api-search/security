---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dinilu.dk
  spf: true
hosts:
- cert_expires: Jan  5 06:18:10 2027 GMT
  host: dinilu.dk
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dinilu Dk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dinilu Reklame- & Trykprodukter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dinilu Reklame- & Trykprodukter
provider_slug: dinilu-dk
slug: dinilu-dk-domain-security
source_filename: dinilu-dk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dinilu.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 06:18:10 2027 GMT\n  hsts: null\ndomains:\n- domain: dinilu.dk\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dinilu-dk/security/dinilu-dk-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Advertising
- Print
- Merchandise
- E-Commerce
- Denmark
---
