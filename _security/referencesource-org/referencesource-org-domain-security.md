---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: referencesource.org
  spf: true
hosts:
- cert_expires: Jan  1 03:13:20 2027 GMT
  host: referencesource.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Referencesource Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for referencesource-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: referencesource-org
provider_slug: referencesource-org
slug: referencesource-org-domain-security
source_filename: referencesource-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: referencesource.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 03:13:20 2027 GMT\n  hsts: false\ndomains:\n- domain: referencesource.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/referencesource-org/security/referencesource-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Data
- Catalog
- Reference
- OpenData
- API
---
