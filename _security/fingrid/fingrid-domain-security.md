---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fingrid.fi
  spf: true
hosts:
- cert_expires: Feb  9 07:58:02 2027 GMT
  host: fingrid.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fingrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fingrid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fingrid
provider_slug: fingrid
slug: fingrid-domain-security
source_filename: fingrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fingrid.fi\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  9 07:58:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fingrid.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fingrid/security/fingrid-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Energy
- Electricity
- Transmission
- Finland
---
