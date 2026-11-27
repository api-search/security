---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: outcomeci.com
  spf: true
hosts:
- cert_expires: Mar 24 23:59:59 2027 GMT
  host: outcomeci.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OutcomeCI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OutcomeCI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OutcomeCI
provider_slug: outcomeci-com
slug: outcomeci-com-domain-security
source_filename: outcomeci-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outcomeci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 24 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: outcomeci.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/outcomeci-com/security/outcomeci-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Security
- Privacy
- Productivity
---
