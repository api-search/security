---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: volunteermatrix.com
  spf: true
hosts:
- cert_expires: Dec 31 07:59:50 2026 GMT
  host: volunteermatrix.com
  hsts: true
  hsts_max_age: 7200
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Volunteer Matrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Volunteer Matrix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Volunteer Matrix
provider_slug: volunteer-matrix
slug: volunteer-matrix-domain-security
source_filename: volunteer-matrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: volunteermatrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 07:59:50 2026 GMT\n  hsts: true\n  hsts_max_age: 7200\ndomains:\n- domain: volunteermatrix.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/volunteer-matrix/security/volunteer-matrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Volunteer Management
- SaaS
- Nonprofit
- Community
- Platform
---
