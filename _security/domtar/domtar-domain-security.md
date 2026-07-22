---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: domtar.com
  spf: true
hosts:
- cert_expires: Sep 25 09:19:28 2026 GMT
  host: www.domtar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Domtar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Domtar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Domtar
provider_slug: domtar
slug: domtar-domain-security
source_filename: domtar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.domtar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 09:19:28 2026 GMT\n  hsts: false\ndomains:\n- domain: domtar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domtar/refs/heads/main/security/domtar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Forest Products
- Lumber
- Manufacturing
- Packaging
- Paper
- Pulp
- Fortune 500
---
