---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carsforsale.com
  spf: true
hosts:
- cert_expires: May 14 23:59:59 2027 GMT
  host: carsforsale.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carsforsale.com® Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carsforsale.com®, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carsforsale.com®
provider_slug: carsforsale
slug: carsforsale-domain-security
source_filename: carsforsale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carsforsale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: carsforsale.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/carsforsale/security/carsforsale-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Marketplace
- Vehicles
- Car Buying
- Financing
---
