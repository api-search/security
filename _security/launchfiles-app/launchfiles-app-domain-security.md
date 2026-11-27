---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: launchfiles.app
  spf: true
hosts:
- cert_expires: Feb 10 04:52:44 2027 GMT
  host: launchfiles.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Launchfiles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Launchfiles, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Launchfiles
provider_slug: launchfiles-app
slug: launchfiles-app-domain-security
source_filename: launchfiles-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: launchfiles.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 04:52:44 2027 GMT\n  hsts: false\ndomains:\n- domain: launchfiles.app\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/launchfiles-app/security/launchfiles-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Software-as-a-Service
- Marketing
- Customer Acquisition
- No-Code
---
