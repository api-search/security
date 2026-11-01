---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: may-sante.com
  spf: true
hosts:
- cert_expires: Jan 16 00:40:40 2027 GMT
  host: may-sante.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: May Sante Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for May, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: May
provider_slug: may-sante-com
slug: may-sante-com-domain-security
source_filename: may-sante-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: may-sante.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 00:40:40 2027 GMT\n  hsts: false\ndomains:\n- domain: may-sante.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/may-sante-com/security/may-sante-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Parenting
- DigitalHealth
- AI
---
