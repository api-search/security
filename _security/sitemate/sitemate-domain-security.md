---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sitemate.com
  spf: true
hosts:
- cert_expires: Jan  6 05:58:17 2027 GMT
  host: sitemate.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sitemate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sitemate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Sitemate
provider_slug: sitemate
slug: sitemate-domain-security
source_filename: sitemate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sitemate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 05:58:17 2027 GMT\n  hsts: false\ndomains:\n- domain: sitemate.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sitemate/security/sitemate-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Construction
- FieldTech
- Automation
- Data Capture
---
