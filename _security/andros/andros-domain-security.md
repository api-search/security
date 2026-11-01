---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: andros.co
  spf: true
hosts:
- cert_expires: Dec  9 18:49:18 2026 GMT
  host: andros.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Andros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Andros, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Andros
provider_slug: andros
slug: andros-domain-security
source_filename: andros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: andros.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 18:49:18 2026 GMT\n  hsts: false\ndomains:\n- domain: andros.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/andros/security/andros-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- ProviderNetwork
- Credentialing
- DataManagement
---
