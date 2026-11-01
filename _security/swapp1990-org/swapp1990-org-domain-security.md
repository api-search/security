---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: swapp1990.org
  spf: true
hosts:
- cert_expires: Dec 19 22:56:22 2026 GMT
  host: swapp1990.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Swapp1990 Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for swapp1990-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: swapp1990-org
provider_slug: swapp1990-org
slug: swapp1990-org-domain-security
source_filename: swapp1990-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swapp1990.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 22:56:22 2026 GMT\n  hsts: false\ndomains:\n- domain: swapp1990.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/swapp1990-org/security/swapp1990-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Technology
- Data
- API
- Placeholder
---
