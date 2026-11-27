---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: sulimerleg.hu
  spf: true
hosts:
- cert_expires: Jan  4 15:08:17 2027 GMT
  host: sulimerleg.hu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SuliMérleg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SuliMérleg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SuliMérleg
provider_slug: sulimerleg-hu
slug: sulimerleg-hu-domain-security
source_filename: sulimerleg-hu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sulimerleg.hu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 15:08:17 2027 GMT\n  hsts: false\ndomains:\n- domain: sulimerleg.hu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/sulimerleg-hu/security/sulimerleg-hu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Data
- Hungary
- Schools
- Rankings
- Company
---
