---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mismo.org
  spf: true
hosts:
- cert_expires: Dec 19 11:46:01 2026 GMT
  host: www.mismo.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mortgage Industry Standards Maintenance Organization Mismo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mortgage Industry Standards Maintenance Organization (MISMO), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mortgage Industry Standards Maintenance Organization (MISMO)
provider_slug: mortgage-industry-standards-maintenance-organization-mismo
slug: mortgage-industry-standards-maintenance-organization-mismo-domain-security
source_filename: mortgage-industry-standards-maintenance-organization-mismo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mismo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 11:46:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mismo.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mortgage-industry-standards-maintenance-organization-mismo/security/mortgage-industry-standards-maintenance-organization-mismo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Mortgage
- Standards
- Data
- Finance
---
