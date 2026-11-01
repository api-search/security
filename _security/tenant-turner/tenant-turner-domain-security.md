---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tenantturner.com
  spf: true
hosts:
- cert_expires: Jan 25 20:26:36 2027 GMT
  host: tenantturner.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tenant Turner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tenant Turner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tenant Turner
provider_slug: tenant-turner
slug: tenant-turner-domain-security
source_filename: tenant-turner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tenantturner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 20:26:36 2027 GMT\n  hsts: false\ndomains:\n- domain: tenantturner.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tenant-turner/security/tenant-turner-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Leasing
- Property-Management
- Automation
- AI
- SaaS
---
