---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tractian.com
  spf: true
hosts:
- cert_expires: Oct 14 19:00:35 2026 GMT
  host: tractian.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 19:00:35 2026 GMT
  host: api.tractian.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tractian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tractian, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tractian
provider_slug: tractian
slug: tractian-domain-security
source_filename: tractian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tractian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 19:00:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tractian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 19:00:35 2026 GMT\n  hsts: null\ndomains:\n- domain: tractian.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tractian/refs/heads/main/security/tractian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Condition Monitoring
- Predictive Maintenance
- CMMS
- Asset Management
- Industrial IoT
- Sensors
- Energy Monitoring
- Manufacturing
---
