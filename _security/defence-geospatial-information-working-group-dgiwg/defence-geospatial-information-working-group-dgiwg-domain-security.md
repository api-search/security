---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dgiwg.org
  spf: true
hosts:
- cert_expires: Dec 23 20:40:11 2026 GMT
  host: www.dgiwg.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Defence Geospatial Information Working Group Dgiwg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defence Geospatial Information Working Group (DGIWG), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Defence Geospatial Information Working Group (DGIWG)
provider_slug: defence-geospatial-information-working-group-dgiwg
slug: defence-geospatial-information-working-group-dgiwg-domain-security
source_filename: defence-geospatial-information-working-group-dgiwg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dgiwg.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 20:40:11 2026 GMT\n  hsts: false\ndomains:\n- domain: dgiwg.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/defence-geospatial-information-working-group-dgiwg/security/defence-geospatial-information-working-group-dgiwg-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geospatial
- Defence
- Standards
- Interoperability
---
