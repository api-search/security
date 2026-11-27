---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: metlex.eu
  spf: true
hosts:
- cert_expires: Jan  3 21:01:33 2027 GMT
  host: metlex.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MetLex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MetLex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MetLex
provider_slug: metlex-eu
slug: metlex-eu-domain-security
source_filename: metlex-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metlex.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 21:01:33 2027 GMT\n  hsts: null\ndomains:\n- domain: metlex.eu\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/metlex-eu/security/metlex-eu-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Compliance
- EU Regulations
- Fintech
- Software-as-a-Service
---
