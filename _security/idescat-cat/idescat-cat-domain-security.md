---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: idescat.cat
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: idescat.cat
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Institut d'Estadística de Catalunya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Institut d''Estadística de Catalunya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Institut d'Estadística de Catalunya
provider_slug: idescat-cat
slug: idescat-cat-domain-security
source_filename: idescat-cat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: idescat.cat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: idescat.cat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/idescat-cat/security/idescat-cat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
