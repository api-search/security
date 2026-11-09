---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: digicatalyst.ca
  spf: true
hosts:
- cert_expires: Feb  2 02:16:47 2027 GMT
  host: digicatalyst.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Digicatalyst Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DigiCatalyst Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DigiCatalyst Systems
provider_slug: digicatalyst-ca
slug: digicatalyst-ca-domain-security
source_filename: digicatalyst-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digicatalyst.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 02:16:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: digicatalyst.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/digicatalyst-ca/security/digicatalyst-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Web Design
- SEO
- Local SEO
- Automation
- Small Business
- Canada
- Toronto
---
