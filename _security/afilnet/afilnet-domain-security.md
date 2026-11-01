---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: afilnet.com
  spf: true
hosts:
- cert_expires: Jan 14 09:01:10 2027 GMT
  host: www.afilnet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Afilnet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Afilnet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Afilnet
provider_slug: afilnet
slug: afilnet-domain-security
source_filename: afilnet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.afilnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 09:01:10 2027 GMT\n  hsts: false\ndomains:\n- domain: afilnet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/afilnet/security/afilnet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Communications
- SMS
- Voice
- Email
- Two Factor
---
