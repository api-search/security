---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mineralstech.com
  spf: true
hosts:
- cert_expires: Sep 24 05:31:40 2026 GMT
  host: www.mineralstech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.mineralstech.com
  https: false
- host: api.mineralstech.com
  https: false
kind: domain-security
layout: security
method: probed
name: Minerals Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Minerals Technologies, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Minerals Technologies
provider_slug: minerals-technologies
slug: minerals-technologies-domain-security
source_filename: minerals-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mineralstech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:31:40 2026 GMT\n  hsts: false\n- host: developer.mineralstech.com\n  https: false\n- host: api.mineralstech.com\n  https: false\ndomains:\n- domain: mineralstech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/minerals-technologies/refs/heads/main/security/minerals-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Specialty Minerals
- Chemical
---
