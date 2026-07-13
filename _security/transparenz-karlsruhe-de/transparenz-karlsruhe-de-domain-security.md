---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: karlsruhe.de
  spf: true
hosts:
- cert_expires: Oct 11 08:54:21 2026 GMT
  host: transparenz.karlsruhe.de
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Transparenz Karlsruhe De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transparency Portal for the City of Karlsruhe, Germany, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Transparency Portal for the City of Karlsruhe, Germany
provider_slug: transparenz-karlsruhe-de
slug: transparenz-karlsruhe-de-domain-security
source_filename: transparenz-karlsruhe-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transparenz.karlsruhe.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 08:54:21 2026 GMT\n  hsts: false\ndomains:\n- domain: karlsruhe.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transparenz-karlsruhe-de/refs/heads/main/security/transparenz-karlsruhe-de-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Germany
---
