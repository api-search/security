---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: protege.com
  spf: false
hosts:
- cert_expires: Dec 26 17:42:12 2026 GMT
  host: www.protege.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Protege Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Protégé, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Protégé
provider_slug: protege-com
slug: protege-com-domain-security
source_filename: protege-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.protege.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 17:42:12 2026 GMT\n  hsts: null\ndomains:\n- domain: protege.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/protege-com/security/protege-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
