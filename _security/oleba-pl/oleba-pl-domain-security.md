---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oleba.pl
  spf: true
hosts:
- cert_expires: Jan 23 20:33:21 2027 GMT
  host: oleba.pl
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ABC Remonty Oleba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ABC Remonty Oleba, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ABC Remonty Oleba
provider_slug: oleba-pl
slug: oleba-pl-domain-security
source_filename: oleba-pl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oleba.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 20:33:21 2027 GMT\n  hsts: false\ndomains:\n- domain: oleba.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oleba-pl/security/oleba-pl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Renovation
- Construction
- Warsaw
- Piaseczno
- Interior Design
---
