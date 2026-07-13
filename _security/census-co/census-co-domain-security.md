---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getcensus.com
  spf: true
hosts:
- cert_expires: Aug 20 00:28:15 2026 GMT
  host: www.getcensus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: developers.getcensus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: app.getcensus.com
  hsts: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Census Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Census, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Census
provider_slug: census-co
slug: census-co-domain-security
source_filename: census-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getcensus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 00:28:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.getcensus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.getcensus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\ndomains:\n- domain: getcensus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/census-co/refs/heads/main/security/census-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Census
- Reverse ETL
- Data Activation
- Embedded
- Audience Hub
- Connect
- Warehouse
- Snowflake
- BigQuery
- Databricks
- Salesforce
- HubSpot
- Marketing
---
