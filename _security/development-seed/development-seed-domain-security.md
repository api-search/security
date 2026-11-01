---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: developmentseed.org
  spf: true
hosts:
- cert_expires: Dec 20 09:16:39 2026 GMT
  host: www.developmentseed.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Development Seed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Development Seed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Development Seed
provider_slug: development-seed
slug: development-seed-domain-security
source_filename: development-seed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.developmentseed.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 09:16:39 2026 GMT\n  hsts: false\ndomains:\n- domain: developmentseed.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/development-seed/security/development-seed-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Geospatial
- DataScience
- OpenSource
- CloudInfrastructure
- AIforEarth
- Company
---
