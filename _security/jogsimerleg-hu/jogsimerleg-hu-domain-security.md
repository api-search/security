---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jogsimerleg.hu
  spf: true
hosts:
- cert_expires: Dec 24 14:00:28 2026 GMT
  host: jogsimerleg.hu
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JogsiMérleg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JogsiMérleg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: JogsiMérleg
provider_slug: jogsimerleg-hu
slug: jogsimerleg-hu-domain-security
source_filename: jogsimerleg-hu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jogsimerleg.hu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 14:00:28 2026 GMT\n  hsts: false\ndomains:\n- domain: jogsimerleg.hu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/jogsimerleg-hu/security/jogsimerleg-hu-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
