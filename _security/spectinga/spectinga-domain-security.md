---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spectinga.com
  spf: true
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: spectinga.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Spectinga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spectinga, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spectinga
provider_slug: spectinga
slug: spectinga-domain-security
source_filename: spectinga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spectinga.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: spectinga.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/spectinga/security/spectinga-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marketplace
- Agriculture
- Construction
- Machinery
- B2B
---
