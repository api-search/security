---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kloudconnectors.com
  spf: true
hosts:
- cert_expires: Jan 13 17:56:24 2027 GMT
  host: kloudconnectors.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kloudconnectors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KloudConnectors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: KloudConnectors
provider_slug: kloudconnectors
slug: kloudconnectors-domain-security
source_filename: kloudconnectors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kloudconnectors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 17:56:24 2027 GMT\n  hsts: false\ndomains:\n- domain: kloudconnectors.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kloudconnectors/security/kloudconnectors-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Integration
- Automation
- Cloud
- Enterprise
- Software-as-a-Service
- Company
---
