---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: egenesisbio.com
  spf: true
hosts:
- cert_expires: Oct  7 18:09:15 2026 GMT
  host: egenesisbio.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Egenesis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eGenesis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: eGenesis
provider_slug: egenesis
slug: egenesis-domain-security
source_filename: egenesis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: egenesisbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 18:09:15 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: egenesisbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/egenesis/refs/heads/main/security/egenesis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotech
- Xenotransplantation
- Gene Editing
- Genome Engineering
- Organ Transplantation
- Life Sciences
- Healthcare
---
