---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: askakil.ai
  spf: true
hosts:
- cert_expires: Jan 16 02:21:01 2027 GMT
  host: askakil.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Akil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Akil
provider_slug: askakil-ai
slug: askakil-ai-domain-security
source_filename: askakil-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: askakil.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 02:21:01 2027 GMT\n  hsts: false\ndomains:\n- domain: askakil.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/askakil-ai/security/askakil-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Data
- NYC
- Public Records
- Artificial Intelligence
- Government
---
