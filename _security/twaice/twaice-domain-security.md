---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: twaice.com
  spf: true
hosts:
- cert_expires: Oct 14 17:03:27 2026 GMT
  host: www.twaice.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Twaice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twaice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Twaice
provider_slug: twaice
slug: twaice-domain-security
source_filename: twaice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.twaice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:03:27 2026 GMT\n  hsts: null\ndomains:\n- domain: twaice.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twaice/refs/heads/main/security/twaice-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Climate
- Batteries
- Battery Analytics
- Energy Storage
- Electric Vehicles
- Energy
- Predictive Analytics
- SaaS
---
