---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meipharma.com
  spf: true
hosts:
- cert_expires: Dec 17 20:28:34 2026 GMT
  host: www.meipharma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mei Pharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MEI Pharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MEI Pharma
provider_slug: mei-pharma
slug: mei-pharma-domain-security
source_filename: mei-pharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meipharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 20:28:34 2026 GMT\n  hsts: false\ndomains:\n- domain: meipharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mei-pharma/security/mei-pharma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- biotech
- pharma
- investment
- therapeutics
- digital-health
---
