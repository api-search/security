---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lume.living
  spf: true
hosts:
- cert_expires: Jan 11 01:06:24 2027 GMT
  host: lume.living
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: naidraug Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for naidraug, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: naidraug
provider_slug: lume-living
slug: lume-living-domain-security
source_filename: lume-living-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lume.living\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 01:06:24 2027 GMT\n  hsts: false\ndomains:\n- domain: lume.living\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lume-living/security/lume-living-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Safety
- Mobile
- Privacy
- Android
---
