---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:info@appraisily.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: appraisily.com
  spf: true
hosts:
- cert_expires: Jan  3 20:57:41 2027 GMT
  host: appraisily.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Appraisily Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appraisily, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Appraisily
provider_slug: appraisily-com
slug: appraisily-com-domain-security
source_filename: appraisily-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appraisily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 20:57:41 2027 GMT\n  hsts: false\ndomains:\n- domain: appraisily.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:info@appraisily.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/appraisily-com/security/appraisily-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Art
- Antiques
- Appraisal
- Valuation
- E-Commerce
---
