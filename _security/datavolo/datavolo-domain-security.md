---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: datavolo.io
  spf: true
hosts:
- cert_expires: Oct  5 02:26:02 2026 GMT
  host: datavolo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datavolo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datavolo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Datavolo
provider_slug: datavolo
slug: datavolo-domain-security
source_filename: datavolo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datavolo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 02:26:02 2026 GMT\n  hsts: false\ndomains:\n- domain: datavolo.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datavolo/refs/heads/main/security/datavolo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Data Pipelines
- Dataflow
- Apache NiFi
- Unstructured Data
- Generative AI
- Data Engineering
- Data Lineage
- ETL
- Snowflake
---
