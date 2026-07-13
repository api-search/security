---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: montreal.ca
  spf: true
hosts:
- cert_expires: Sep 12 11:25:15 2026 GMT
  host: donnees.montreal.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Donnees Montreal Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Donnees Ouvertes Montreal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Donnees Ouvertes Montreal
provider_slug: donnees-montreal-ca
slug: donnees-montreal-ca-domain-security
source_filename: donnees-montreal-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: donnees.montreal.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 11:25:15 2026 GMT\n  hsts: false\ndomains:\n- domain: montreal.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/donnees-montreal-ca/refs/heads/main/security/donnees-montreal-ca-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Municipal Government
- Canada
---
