---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pharmacompass.com
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.pharmacompass.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bojinbiotechnology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bojinbiotechnology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bojinbiotechnology
provider_slug: bojinbiotechnology
slug: bojinbiotechnology-domain-security
source_filename: bojinbiotechnology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pharmacompass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: pharmacompass.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bojinbiotechnology/refs/heads/main/security/bojinbiotechnology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
