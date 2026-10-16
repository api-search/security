---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: congruencetx.com
  spf: true
hosts:
- cert_expires: Dec 12 13:25:20 2026 GMT
  host: congruencetx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Congruencetherapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Congruencetherapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Congruencetherapeutics
provider_slug: congruencetherapeutics
slug: congruencetherapeutics-domain-security
source_filename: congruencetherapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: congruencetx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 13:25:20 2026 GMT\n  hsts: false\ndomains:\n- domain: congruencetx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/congruencetherapeutics/refs/heads/main/security/congruencetherapeutics-domain-security.yml
summary_line: TLSv1.3
tags:
- Biotechnology
- Therapeutics
---
