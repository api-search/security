---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acrescout.ca
  spf: true
hosts:
- cert_expires: Dec 27 18:25:48 2026 GMT
  host: acrescout.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AcreScout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AcreScout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AcreScout
provider_slug: acrescout-ca
slug: acrescout-ca-domain-security
source_filename: acrescout-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acrescout.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 18:25:48 2026 GMT\n  hsts: false\ndomains:\n- domain: acrescout.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/acrescout-ca/security/acrescout-ca-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Canada
- Land Listings
- Data Aggregation
- Open Data
---
