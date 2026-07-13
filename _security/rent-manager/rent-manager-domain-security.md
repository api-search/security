---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rentmanager.com
  spf: true
hosts:
- cert_expires: Aug 30 03:05:51 2026 GMT
  host: www.rentmanager.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rent Manager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rent Manager, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rent Manager
provider_slug: rent-manager
slug: rent-manager-domain-security
source_filename: rent-manager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rentmanager.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 03:05:51 2026 GMT\n  hsts: false\ndomains:\n- domain: rentmanager.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rent-manager/refs/heads/main/security/rent-manager-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Property Management
- Real Estate
- Tenants
- Leases
- Work Orders
- Accounting
- Maintenance
- Residential
- Commercial
- HOA
- Multifamily
---
