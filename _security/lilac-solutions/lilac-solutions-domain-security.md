---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lilacsolutions.com
  spf: true
hosts:
- cert_expires: Oct  2 05:41:03 2026 GMT
  host: lilacsolutions.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lilac Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lilac Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lilac Solutions
provider_slug: lilac-solutions
slug: lilac-solutions-domain-security
source_filename: lilac-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lilacsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:41:03 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: lilacsolutions.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lilac-solutions/refs/heads/main/security/lilac-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Lithium
- Direct Lithium Extraction
- Ion Exchange
- Critical Minerals
- Battery Materials
- Mining Technology
- Climate Tech
- Energy Transition
- Industrial Hardware
---
