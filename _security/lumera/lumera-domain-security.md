---
description: ''
domains:
- caa:
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lumera.com
  spf: true
hosts:
- cert_expires: Jan  5 13:53:46 2027 GMT
  host: lumera.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lumera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lumera
provider_slug: lumera
slug: lumera-domain-security
source_filename: lumera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 13:53:46 2027 GMT\n  hsts: false\ndomains:\n- domain: lumera.com\n  dnssec: false\n  caa:\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumera/refs/heads/main/security/lumera-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Integration
- API-Management
- Data-Synchronization
- Enterprise
---
