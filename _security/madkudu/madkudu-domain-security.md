---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:maxime.gaudin@madkudu.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: madkudu.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: madkudu.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 22:27:08 2026 GMT
  host: developers.madkudu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: madapi.madkudu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Madkudu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MadKudu, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MadKudu
provider_slug: madkudu
slug: madkudu-domain-security
source_filename: madkudu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: madkudu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\n- host: developers.madkudu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:27:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: madapi.madkudu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: madkudu.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:maxime.gaudin@madkudu.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madkudu/refs/heads/main/security/madkudu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Applicative Saas
- Sales Intelligence
- Lead Scoring
- Predictive Analytics
- Account Intelligence
- Data Enrichment
- MCP
---
