---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sncf.com
  spf: true
hosts:
- cert_expires: Mar 24 23:59:59 2027 GMT
  host: sncf.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sncf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SNCF, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SNCF
provider_slug: sncf
slug: sncf-domain-security
source_filename: sncf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sncf.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sncf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sncf/refs/heads/main/security/sncf-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
---
