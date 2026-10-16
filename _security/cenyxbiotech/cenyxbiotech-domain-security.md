---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cenyxbiotech.com
  spf: true
hosts:
- cert_expires: Dec 24 08:30:30 2026 GMT
  host: cenyxbiotech.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cenyxbiotech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cenyxbiotech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cenyxbiotech
provider_slug: cenyxbiotech
slug: cenyxbiotech-domain-security
source_filename: cenyxbiotech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cenyxbiotech.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 08:30:30 2026 GMT\n  hsts: false\ndomains:\n- domain: cenyxbiotech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cenyxbiotech/refs/heads/main/security/cenyxbiotech-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
---
