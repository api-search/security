---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: firefly-iii.org
  spf: true
hosts:
- cert_expires: Dec 31 07:23:19 2026 GMT
  host: firefly-iii.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firefly Iii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firefly III, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Firefly III
provider_slug: firefly-iii
slug: firefly-iii-domain-security
source_filename: firefly-iii-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firefly-iii.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 07:23:19 2026 GMT\n  hsts: null\ndomains:\n- domain: firefly-iii.org\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/firefly-iii/security/firefly-iii-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Finance
- OpenSource
- PersonalFinance
- Budgeting
- Community
---
