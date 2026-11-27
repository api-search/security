---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bullpenstrategygroup.com
  spf: true
hosts:
- cert_expires: Jan 18 00:09:33 2027 GMT
  host: bullpenstrategygroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bullpen Strategy Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bullpen Strategy Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bullpen Strategy Group
provider_slug: bullpenstrategygroup-com
slug: bullpenstrategygroup-com-domain-security
source_filename: bullpenstrategygroup-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bullpenstrategygroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 00:09:33 2027 GMT\n  hsts: false\ndomains:\n- domain: bullpenstrategygroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bullpenstrategygroup-com/security/bullpenstrategygroup-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advisory
- Strategic
- Communications
- Artificial Intelligence
---
