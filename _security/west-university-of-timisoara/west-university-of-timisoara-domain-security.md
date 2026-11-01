---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: uvt.ro
  spf: true
hosts:
- cert_expires: Dec 17 12:54:02 2026 GMT
  host: www.uvt.ro
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: West University Of Timisoara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for West University of Timisoara, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: West University of Timisoara
provider_slug: west-university-of-timisoara
slug: west-university-of-timisoara-domain-security
source_filename: west-university-of-timisoara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uvt.ro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 12:54:02 2026 GMT\n  hsts: false\ndomains:\n- domain: uvt.ro\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/west-university-of-timisoara/security/west-university-of-timisoara-domain-security.yml
summary_line: TLSv1.3
tags:
- Education
- University
- Romania
- Research
- Public
---
